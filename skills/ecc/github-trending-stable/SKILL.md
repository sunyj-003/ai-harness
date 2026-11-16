---
name: github-trending-stable
description: "通过网页抓取获取 GitHub 按日/周/月增长的热门仓库。当用户询问 GitHub 趋势、热门项目、本周热点或「什么在 GitHub 上 trending」时使用。可输出列表或 JSON，无需 API Key。"
---

# GitHub Trending

抓取 GitHub 按日/周/月增长的热门仓库，仅使用 Python 标准库，无需安装第三方包。

## 何时使用

- 用户询问 **GitHub 趋势**、**热门项目**、**本周热点**
- 用户需要 **今日** / **本周** / **本月** 趋势
- 用户需要按 **编程语言** 筛选的 trending

## 快速开始（推荐方案：正则解析 HTML）

### ⚠️ 本地脚本已废弃
脚本 `scripts/github_trending.py` 已废弃，请使用以下方式直接抓取。

### execute_code（推荐，沙盒和 host 均可用）

```python
import subprocess, re

# Fetch trending page
headers = [
    'User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36',
    'Accept-Language: en-US,en;q=0.9',
]
hdr_args = []
for h in headers:
    hdr_args += ['-H', h]

# weekly: ?since=weekly, monthly: ?since=monthly, daily: 默认（无参数）
url = "https://github.com/trending?since=weekly"
result = subprocess.run(
    ['curl', '-s', '--max-time', '20', '--compressed'] + hdr_args + [url],
    capture_output=True, text=True, timeout=25
)
html_content = result.stdout

# 解析每个 Box-row article
articles = re.findall(r'<article[^>]*class="Box-row"[^>]*>(.*?)</article>',
                      html_content, re.DOTALL)

repos = []
for body in articles:
    r = {}
    # 仓库名和 URL：h2 > a href="/owner/repo"
    h2_match = re.search(r'<h2[^>]*>(.*?)</h2>', body, re.DOTALL)
    if h2_match:
        hrefs = re.findall(r'href="(/[a-zA-Z0-9_\-\.]+/[a-zA-Z0-9_\-\.]+)"', h2_match.group(1))
        for href in hrefs:
            parts = href.lstrip('/').split('/')
            if len(parts) == 2 and parts[0] not in ('login', 'sponsors', 'notifications', 'account', 'settings'):
                r['full_name'] = f"{parts[0]}/{parts[1]}"
                r['url'] = 'https://github.com/' + r['full_name']
                break
    # 描述：p.col-9 或 p.color-fg-muted
    desc_match = re.search(r'<p[^>]*col-9[^>]*>(.*?)</p>', body, re.DOTALL)
    if desc_match:
        r['description'] = re.sub(r'<[^>]+>', '', desc_match.group(1)).strip()
    # 编程语言
    lang_match = re.search(r'<span[^>]*itemprop="programmingLanguage"[^>]*>(.*?)</span>', body, re.DOTALL)
    r['language'] = lang_match.group(1).strip() if lang_match else ''
    # 总 stars
    stars_match = re.search(r'aria-label="([\d,]+) star[s]?', body)
    r['stars_total'] = stars_match.group(1).replace(',', '') if stars_match else ''
    # 本周/今日新增 stars
    gained_match = re.search(r'([\d,]+)\s*stars?\s*(today|this week|this month)', body, re.IGNORECASE)
    if gained_match:
        r['stars_gained'] = gained_match.group(1).replace(',', '')
        r['gained_period'] = gained_match.group(2)
    if r.get('full_name'):
        repos.append(r)
```

### 终端方案
```bash
curl -s --max-time 20 -H "User-Agent: Mozilla/5.0" \
  "https://github.com/trending?since=weekly" > /tmp/trending.html
```
然后用 Python 脚本解析 `/tmp/trending.html`。

## 已知环境问题
- **⚠️ weekly 页面不返回总 star 数**：每日趋势页有 `aria-label="X stars"` 和 `aria-label="X forks"`，但每周/每月趋势页**只有新增星数**，无总星数。
- 沙盒环境（execute_code）**可以**直接抓取 GitHub trending 页面（测试通过），无需 GitHub API。
- 每周页面至少返回 10 个仓库，建议合并日榜补充数据。

## 参数说明

| 参数 | 取值 | 默认 | 说明 |
|------|------|------|------|
| `period` | `daily`, `weekly`, `monthly` | `weekly` | 统计「新增 star」的时间范围 |
| `--limit` | 整数 | 15 | 返回仓库数量上限 |
| `--language` | 字符串 | 全部 | 按语言筛选（见下方） |
| `--json` | 开关 | — | 输出 JSON 而非可读文本 |

**语言**：可用全称或别名。脚本支持别名：`py`→python、`ts`→typescript、`js`→javascript、`cpp`/`c++`→c++、`c#`/`csharp`→c#、`rs`→rust、`rb`→ruby、`go`→go。其他按原样传入（如 `--language "c"`）。

## 输出格式

### 文本（默认）

- 排名、仓库 `full_name`、描述（最多 90 字）
- 每行统计符号含义：
  - **🔧** 编程语言
  - **⭐** 总 Star 数
  - **📈** 本周期新增 Star 数
- 时间为北京时区 (UTC+8)

### JSON（`--json`）

```json
{
  "period": "weekly",
  "updated_at": "2026-03-13T21:00:00+08:00",
  "data": [
    {
      "rank": 1,
      "full_name": "owner/repo",
      "url": "https://github.com/owner/repo",
      "description": "...",
      "language": "Python",
      "stars_total": "12345",
      "stars_gained": 1234
    }
  ]
}
```

## 数据来源

- **地址**：`https://github.com/trending`（日）/ `?since=weekly`（周）/ `?since=monthly`（月）
- **方式**：正则表达式解析 HTML 页面（无需浏览器、无需登录、无需 API Key）
- **实时**：每次执行都会拉取当前页面

## 依赖

仅使用 Python 标准库：`re`、`subprocess`、`json`、`datetime`。**无需 pip 安装。**

### 常见问题

| 现象 | 处理建议 |
|------|----------|
| 返回空列表 / 无仓库 | 可能是网络提前断开（IncompleteRead）。重试；若脚本支持，可改用分块读取。 |
| 解析报错 / 结构不对 | GitHub 可能改版了页面结构，需更新脚本选择器或解析逻辑。当前验证选择器：`Box-row`、`col-9`、`itemprop="programmingLanguage"`、`aria-label="X stars"` |
| 超时 | 检查网络；默认超时 20 秒。 |
| Windows 控制台 emoji 乱码/报错 | 设置 `PYTHONIOENCODING=utf-8` 或使用 `--json` 在别处解析。 |
| **HTTP 529** | GitHub 服务集群负载高（限流），稍后重试。建议 cron 任务增加重试逻辑。 |
| weekly/monthly 页面总 star 为空 | 正常行为——GitHub 周榜/月榜页面只显示本周期新增 star 数，不显示仓库总 star 数。日榜两者都有。 |

## 说明

- 趋势按**选定周期内新增的 star** 排序，不是按总 star 数。
- 若需 GitHub API（如按 star 搜索、鉴权等），请使用单独的 GitHub API 类技能。
