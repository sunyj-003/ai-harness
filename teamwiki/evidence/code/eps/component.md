---
title: eps component
domain: code-knowledge
source:
  - gateway/src/main/java/com/findsoft/education/gateway/GatewayServerApplication.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/InfraServerApplication.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/SecmanStudentServiceApplication.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/dialoguerecord/AiDialogueContextService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicator/AbstractIndicatorPreviewService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/DataPermissionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/person/AigcSemanticMatchService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/ref/ReferenceCheckService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantCaseAssignmentService.java
  - framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/datacopy/TenantDataCopyService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/job/JobController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiAccessLogController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/redis/RedisController.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppEventController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentRankListController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppGroupMemberCharacterController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppOrgController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppPeriodNotificationController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/report/AppReportController.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/thirdparty/CrwPlatformAppController.java
  - system/.claude/worktrees/agent-a05d15f3422c62fcc/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-a21c10cea4cc3f423/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-a7325805457b97091/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-a8dfe6b2786c17159/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-a97b2dc46b17dc0e7/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-a98b9d97d86021fe5/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-ab0078566444831a0/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-ad541c8721675ff73/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/.claude/worktrees/agent-ae591e3afc4f955a4/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/captcha/CaptchaController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java
---

# Component

- `GatewayServerApplication` ← gateway/src/main/java/com/findsoft/education/gateway/GatewayServerApplication.java:7 [EXTRACTED]
  ```
  public class GatewayServerApplication {
  ```
- `InfraServerApplication` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/InfraServerApplication.java:16 [EXTRACTED]
  ```
  public class InfraServerApplication {
  ```
- `SecmanStudentServiceApplication` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/SecmanStudentServiceApplication.java:13 [EXTRACTED]
  ```
  public class SecmanStudentServiceApplication {
  ```
- `SystemServerApplication` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `AigcService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcService.java:35 [EXTRACTED]
  ```
  public class AigcService {
  ```
- `@Service:AigcService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcService.java:35 [EXTRACTED]
  ```
  public class AigcService {
  ```
- `AiDialogueContextService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/dialoguerecord/AiDialogueContextService.java:37 [EXTRACTED]
  ```
  public class AiDialogueContextService {
  ```
- `@Service:AiDialogueContextService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/dialoguerecord/AiDialogueContextService.java:37 [EXTRACTED]
  ```
  public class AiDialogueContextService {
  ```
- `AbstractIndicatorPreviewService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicator/AbstractIndicatorPreviewService.java:48 [EXTRACTED]
  ```
  public abstract class AbstractIndicatorPreviewService {
  ```
- `DataPermissionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/DataPermissionService.java:23 [EXTRACTED]
  ```
  public class DataPermissionService {
  ```
- `@Service:DataPermissionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/DataPermissionService.java:23 [EXTRACTED]
  ```
  public class DataPermissionService {
  ```
- `AigcSemanticMatchService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/person/AigcSemanticMatchService.java:27 [EXTRACTED]
  ```
  public class AigcSemanticMatchService {
  ```
- `@Service:AigcSemanticMatchService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/person/AigcSemanticMatchService.java:27 [EXTRACTED]
  ```
  public class AigcSemanticMatchService {
  ```
- `ReferenceCheckService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/ref/ReferenceCheckService.java:20 [EXTRACTED]
  ```
  public class ReferenceCheckService {
  ```
- `@Service:ReferenceCheckService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/ref/ReferenceCheckService.java:20 [EXTRACTED]
  ```
  public class ReferenceCheckService {
  ```
- `TenantCaseAssignmentService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantCaseAssignmentService.java:10 [EXTRACTED]
  ```
  public class TenantCaseAssignmentService {
  ```
- `@Service:TenantCaseAssignmentService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantCaseAssignmentService.java:10 [EXTRACTED]
  ```
  public class TenantCaseAssignmentService {
  ```
- `TenantDataCopyService` ← framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/datacopy/TenantDataCopyService.java:31 [EXTRACTED]
  ```
  public class TenantDataCopyService {
  ```
- `@Service:TenantDataCopyService` ← framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/datacopy/TenantDataCopyService.java:31 [EXTRACTED]
  ```
  public class TenantDataCopyService {
  ```
- `CodegenController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:45 [EXTRACTED]
  ```
  public class CodegenController {
  ```
- `ConfigController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:36 [EXTRACTED]
  ```
  public class ConfigController {
  ```
- `DataSourceConfigController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:26 [EXTRACTED]
  ```
  public class DataSourceConfigController {
  ```
- `FileConfigController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:27 [EXTRACTED]
  ```
  public class FileConfigController {
  ```
- `FileController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:39 [EXTRACTED]
  ```
  public class FileController {
  ```
- `JobController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/job/JobController.java:18 [EXTRACTED]
  ```
  public class JobController {
  ```
- `ApiAccessLogController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiAccessLogController.java:34 [EXTRACTED]
  ```
  public class ApiAccessLogController {
  ```
- `ApiErrorLogController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java:35 [EXTRACTED]
  ```
  public class ApiErrorLogController {
  ```
- `RedisController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/redis/RedisController.java:24 [EXTRACTED]
  ```
  public class RedisController {
  ```
- `AppFileController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java:28 [EXTRACTED]
  ```
  public class AppFileController {
  ```
- `CaseSnapController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:39 [EXTRACTED]
  ```
  public class CaseSnapController {
  ```
- `ExperimentController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:31 [EXTRACTED]
  ```
  public class ExperimentController {
  ```
- `GroupController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:31 [EXTRACTED]
  ```
  public class GroupController {
  ```
- `GroupMemberController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:28 [EXTRACTED]
  ```
  public class GroupMemberController {
  ```
- `GroupTemplateController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:31 [EXTRACTED]
  ```
  public class GroupTemplateController {
  ```
- `JudgeController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:34 [EXTRACTED]
  ```
  public class JudgeController {
  ```
- `RankListController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:37 [EXTRACTED]
  ```
  public class RankListController {
  ```
- `ReportController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:28 [EXTRACTED]
  ```
  public class ReportController {
  ```
- `ReportGroupController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:28 [EXTRACTED]
  ```
  public class ReportGroupController {
  ```
- `CrwPlatformController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java:39 [EXTRACTED]
  ```
  public class CrwPlatformController {
  ```
- `AppApprovalController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:26 [EXTRACTED]
  ```
  public class AppApprovalController {
  ```
- `DialogueRecordController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:38 [EXTRACTED]
  ```
  public class DialogueRecordController {
  ```
- `AppEventController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppEventController.java:27 [EXTRACTED]
  ```
  public class AppEventController {
  ```
- `AppExperimentController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:33 [EXTRACTED]
  ```
  public class AppExperimentController {
  ```
- `AppExperimentFunctionController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:30 [EXTRACTED]
  ```
  public class AppExperimentFunctionController {
  ```
- `AppExperimentGroupController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:32 [EXTRACTED]
  ```
  public class AppExperimentGroupController {
  ```
- `AppExperimentIndicatorController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:33 [EXTRACTED]
  ```
  public class AppExperimentIndicatorController {
  ```
- `AppExperimentMemberController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:30 [EXTRACTED]
  ```
  public class AppExperimentMemberController {
  ```
- `AppExperimentPersonController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java:29 [EXTRACTED]
  ```
  public class AppExperimentPersonController {
  ```
- `AppExperimentRankListController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentRankListController.java:47 [EXTRACTED]
  ```
  public class AppExperimentRankListController {
  ```
- `AppExperimentScoreTestController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:40 [EXTRACTED]
  ```
  public class AppExperimentScoreTestController {
  ```
- `AppGroupMemberCharacterController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppGroupMemberCharacterController.java:25 [EXTRACTED]
  ```
  public class AppGroupMemberCharacterController {
  ```
- `AppOrgController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppOrgController.java:30 [EXTRACTED]
  ```
  public class AppOrgController {
  ```
- `AppPeriodNotificationController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppPeriodNotificationController.java:29 [EXTRACTED]
  ```
  public class AppPeriodNotificationController {
  ```
- `AppReportController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/report/AppReportController.java:31 [EXTRACTED]
  ```
  public class AppReportController {
  ```
- `CrwPlatformAppController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/thirdparty/CrwPlatformAppController.java:39 [EXTRACTED]
  ```
  public class CrwPlatformAppController {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-a05d15f3422c62fcc/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-a21c10cea4cc3f423/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-a7325805457b97091/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-a8dfe6b2786c17159/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-a97b2dc46b17dc0e7/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-a98b9d97d86021fe5/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-ab0078566444831a0/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-ad541c8721675ff73/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `SystemServerApplication` ← system/.claude/worktrees/agent-ae591e3afc4f955a4/eps-module-system-server/src/main/java/com/findsoft/education/module/system/SystemServerApplication.java:17 [EXTRACTED]
  ```
  public class SystemServerApplication {
  ```
- `AigcConfigController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:31 [EXTRACTED]
  ```
  public class AigcConfigController {
  ```
- `ArchiveController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:31 [EXTRACTED]
  ```
  public class ArchiveController {
  ```
- `AssessController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:31 [EXTRACTED]
  ```
  public class AssessController {
  ```
- `AuthController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:68 [EXTRACTED]
  ```
  public class AuthController {
  ```
- `BusinessBindController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:35 [EXTRACTED]
  ```
  public class BusinessBindController {
  ```
- `BusinessController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:33 [EXTRACTED]
  ```
  public class BusinessController {
  ```
- `BusinessInstitutionController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:38 [EXTRACTED]
  ```
  public class BusinessInstitutionController {
  ```
- `CaptchaController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/captcha/CaptchaController.java:22 [EXTRACTED]
  ```
  public class CaptchaController {
  ```
- `CaseArrangementController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:33 [EXTRACTED]
  ```
  public class CaseArrangementController {
  ```
- `CaseBusinessBindController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:34 [EXTRACTED]
  ```
  public class CaseBusinessBindController {
  ```
- `CaseBusinessFunctionController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:31 [EXTRACTED]
  ```
  public class CaseBusinessFunctionController {
  ```
- `CaseGridController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:33 [EXTRACTED]
  ```
  public class CaseGridController {
  ```