---
title: eps error
domain: code-knowledge
source:
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsSendService.java
  - framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/datacopy/TenantDataCopyService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java
---

# Error

- `IllegalArgumentException` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcService.java:206 [EXTRACTED]
  ```
  throw new IllegalArgumentException("沟通技巧批量评分参数不完整");
  ```
- `UnsupportedOperationException` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsSendService.java:58 [EXTRACTED]
  ```
  throw new UnsupportedOperationException("暂时不支持该操作，感兴趣可以实现该功能哟！");
  ```
- `IllegalArgumentException` ← framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/datacopy/TenantDataCopyService.java:101 [EXTRACTED]
  ```
  throw new IllegalArgumentException("无效的SQL条件参数，可能存在SQL注入风险: " + condition);
  ```
- `RuntimeException` ← framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/datacopy/TenantDataCopyService.java:231 [EXTRACTED]
  ```
  throw new RuntimeException(e);
  ```
- `IllegalArgumentException` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:97 [EXTRACTED]
  ```
  throw new IllegalArgumentException("结尾的 path 路径必须传递");
  ```