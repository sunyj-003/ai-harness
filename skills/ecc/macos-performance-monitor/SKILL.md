---
name: macos-performance-monitor
description: "macOS 性能监控定时任务 — 监控 CPU/内存/交换/WD/磁盘，通过微信推送报告"
tags: [macOS, monitoring, cron, performance]
version: 1.0.0
---

# macOS 性能监控

通过 cron job 每 2 小时收集 macOS 系统指标，通过微信推送报告。

## 监控指标

| 指标 | 告警阈值 |
|------|---------|
| 交换内存 | > 500MB |
| 可用内存 | < 2GB |
| WindowServer CPU | > 10% |
| 视频壁纸扩展 | 运行中 |
| pap.er 壁纸应用 | 运行中 |
| 磁盘剩余 | < 15% |

## 监控脚本

路径: `~/.hermes/scripts/performance-monitor.sh`

### 关键调试经验 (避免踩坑)

**vm_stat page size 输出格式带前缀：**
```bash
# 错误：会捕获 "4096 bytes)" 导致算术报错
PAGE_SIZE=$(vm_stat | grep "page size" | awk '{print $NF}')

# 正确：提取 "of" 后面的数字
PAGE_SIZE=$(vm_stat | grep "page size" | sed 's/.*of //' | awk '{print $1}')
```

**Pages free 用 awk 模式匹配，避免空匹配：**
```bash
# 错误：管道 grep 可能无输出，导致后续 $NF 为空
PAGES_FREE=$(vm_stat | grep "Pages free" | awk '{gsub(/\./,"",$NF); print $NF}')

# 正确：用 awk 模式匹配
PAGES_FREE=$(vm_stat | awk '/Pages free/{gsub(/\./,"",$NF); print $NF}')
```

**sysctl vm.swapusage 多字段解析：**
```bash
# 输出格式：total = 4096.00M  used = 2963.00M  free = 1133.00M  (encrypted)
# 用 grep -o 配合 sed 精确提取
SWAP_USED=$(sysctl -n vm.swapusage | grep -o '[0-9]*\.[0-9]*M' | sed -n '2p' | tr -d 'M' | cut -d. -f1)
SWAP_TOTAL=$(sysctl -n vm.swapusage | grep -o '[0-9]*\.[0-9]*M' | sed -n '1p' | tr -d 'M' | cut -d. -f1)
```

**WindowServer CPU 可能为空：**
```bash
# 错误：空字符串时 ${WS_CPU%.*} 报错
WS_INT=${WS_CPU%.*}

# 正确：显式提取整数部分
WS_INT=$(echo "$WS_CPU" | grep -o '^[0-9]*' | head -1)
```

## 常见高占用进程

| 进程 | 原因 | 解决 |
|------|------|------|
| WallpaperVideoExtension | 视频壁纸系统扩展 | 设为静态壁纸后 kill PID |
| pap.er | 第三方壁纸应用 | 退出应用 |
| HexinStockFreeWidgetExtension | 同花顺股票插件 | kill PID |
| CleanMyMac5.HealthMonitor | CleanMyMac 健康监控 | launchctl unload |
| WindowServer > 15% | 视频壁纸 / 外接显示器 / Retina | 关闭视频壁纸，降低分辨率 |

## Cron Job 创建

```bash
# 监控脚本
~/.hermes/scripts/performance-monitor.sh

# cron job (每2小时)
# deliver=weixin:o9cq804I-cRMm3RXTYMhU-nvvXjg@im.wechat
```

## 已知问题

- 磁盘剩余 12% 是 Boot Camp 分区的警告，不影响系统
- WindowServer 在 Retina 屏幕上本身就有 5-15% 基础占用
- 16GB 内存 + i7-8750H 在视频播放时交换内存 2GB 左右属正常范围
