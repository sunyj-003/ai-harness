---
title: eps interface
domain: code-knowledge
source:
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/codegen/CodegenService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/config/ConfigService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/db/DatabaseTableService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/db/DataSourceConfigService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/file/FileConfigService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/file/FileService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/logger/ApiAccessLogService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/logger/ApiErrorLogService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcConfigService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/dialoguerecord/DialogueRecordService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AnswerRecordService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppExperimentFunctionService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppExperimentPersonService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppExperimentService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppOrgService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppPeriodNotificationService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/CaseSnapService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ElderlyRedistributionService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/EventLifecycleService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ExperimentLifecycleService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ExperimentService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ExpEventService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupIndicatorService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupMemberAccessService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupMemberCharacterService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupMemberService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupTemplateService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/JudgeService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PeriodScheduleService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PersonBusinessService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PersonIndicatorValueService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PersonService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/rank/RankListItemService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/rank/RankListService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/report/ReportGroupService.java
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/report/ReportService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/aigc/AigcConfigService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/archive/ArchiveService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/assess/AssessService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/auth/AdminAuthService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessBindService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessInstitutionFileService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessInstitutionQuestionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseArrangementService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseBusinessFunctionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseBusinessService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseExperimentModeService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseGridService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseInfoService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseInstitutionFileService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseInstitutionQuestionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseOrgService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseSnapshotService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseWeightService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/casequestion/CaseQuestionPreviewService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/category/CategoryService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/character/CharacterService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/clazz/ClazzService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/crwplatform/CrwPlatformService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dept/DeptService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dept/PostService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dialoguematerial/DialogueMaterialService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dialoguesynonym/DialogueSynonymService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dict/DictDataService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dict/DictTypeService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/file/FileService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/function/FunctionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicator/IndicatorCategoryService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicator/IndicatorService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplate/CaseEvalIndicatorService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplate/IndicatorTemplatePreviewService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplate/IndicatorTemplateService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplatecategory/IndicatorTemplateCategoryService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplateindicator/IndicatorTemplateIndicatorService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplateindicator/IndicatorTemplateIndicatorWeightService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/institution/InstitutionFileService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/institution/InstitutionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/logger/LoginLogService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/logger/OperateLogService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailAccountService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailLogService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailSendService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailTemplateService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/member/MemberService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notice/NoticeService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notify/NotifyMessageService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notify/NotifySendService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notify/NotifyTemplateService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2ApproveService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2ClientService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2CodeService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2GrantService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2TokenService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/operate/OperateService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/org/OrgService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/MenuService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/PermissionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/RoleService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/person/PersonService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/persondialoguematerial/PersonDialogueMaterialService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/personindicatorvalue/PersonIndicatorValueService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/portal/FeedbackService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/portal/PortalService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/portal/TrialApplicationService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdArrangementService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdGridService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdOrgService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProductService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdWeightService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/question/QuestionOptionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/question/QuestionService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsChannelService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsCodeService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsLogService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsSendService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsTemplateService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/social/SocialClientService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/social/SocialUserService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantPackageService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenantsyncsnapshot/TenantSyncSnapshotService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/user/AdminUserService.java
  - system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/userclazz/UserClazzService.java
  - framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/service/TenantFrameworkService.java
  - framework/eps-framework/eps-spring-boot-starter-security/src/main/java/com/findsoft/education/framework/security/core/service/SecurityFrameworkService.java
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
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/demo/demo01/Demo01ContactService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/demo/demo02/Demo02CategoryService.java
  - infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/demo/demo03/Demo03StudentService.java
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
  - secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/framework/mq/service/MqMessageService.java
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

# Interface

- `CodegenService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/codegen/CodegenService.java:19 [EXTRACTED]
  ```
  public interface CodegenService {
  ```
- `ConfigService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/config/ConfigService.java:16 [EXTRACTED]
  ```
  public interface ConfigService {
  ```
- `DatabaseTableService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/db/DatabaseTableService.java:12 [EXTRACTED]
  ```
  public interface DatabaseTableService {
  ```
- `DataSourceConfigService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/db/DataSourceConfigService.java:14 [EXTRACTED]
  ```
  public interface DataSourceConfigService {
  ```
- `FileConfigService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/file/FileConfigService.java:16 [EXTRACTED]
  ```
  public interface FileConfigService {
  ```
- `FileService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/file/FileService.java:17 [EXTRACTED]
  ```
  public interface FileService {
  ```
- `ApiAccessLogService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/logger/ApiAccessLogService.java:13 [EXTRACTED]
  ```
  public interface ApiAccessLogService {
  ```
- `ApiErrorLogService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/logger/ApiErrorLogService.java:13 [EXTRACTED]
  ```
  public interface ApiErrorLogService {
  ```
- `AigcConfigService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/aigc/AigcConfigService.java:12 [EXTRACTED]
  ```
  public interface AigcConfigService {
  ```
- `DialogueRecordService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/dialoguerecord/DialogueRecordService.java:19 [EXTRACTED]
  ```
  public interface DialogueRecordService {
  ```
- `AnswerRecordService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AnswerRecordService.java:14 [EXTRACTED]
  ```
  public interface AnswerRecordService {
  ```
- `AppExperimentFunctionService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppExperimentFunctionService.java:13 [EXTRACTED]
  ```
  public interface AppExperimentFunctionService {
  ```
- `AppExperimentPersonService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppExperimentPersonService.java:12 [EXTRACTED]
  ```
  public interface AppExperimentPersonService {
  ```
- `AppExperimentService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppExperimentService.java:13 [EXTRACTED]
  ```
  public interface AppExperimentService {
  ```
- `AppOrgService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppOrgService.java:12 [EXTRACTED]
  ```
  public interface AppOrgService {
  ```
- `AppPeriodNotificationService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/AppPeriodNotificationService.java:12 [EXTRACTED]
  ```
  public interface AppPeriodNotificationService {
  ```
- `CaseSnapService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/CaseSnapService.java:16 [EXTRACTED]
  ```
  public interface CaseSnapService {
  ```
- `ElderlyRedistributionService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ElderlyRedistributionService.java:12 [EXTRACTED]
  ```
  public interface ElderlyRedistributionService {
  ```
- `EventLifecycleService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/EventLifecycleService.java:11 [EXTRACTED]
  ```
  public interface EventLifecycleService {
  ```
- `ExperimentLifecycleService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ExperimentLifecycleService.java:13 [EXTRACTED]
  ```
  public interface ExperimentLifecycleService {
  ```
- `ExperimentService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ExperimentService.java:18 [EXTRACTED]
  ```
  public interface ExperimentService {
  ```
- `ExpEventService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/ExpEventService.java:13 [EXTRACTED]
  ```
  public interface ExpEventService {
  ```
- `GroupIndicatorService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupIndicatorService.java:22 [EXTRACTED]
  ```
  public interface GroupIndicatorService {
  ```
- `GroupMemberAccessService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupMemberAccessService.java:16 [EXTRACTED]
  ```
  public interface GroupMemberAccessService {
  ```
- `GroupMemberCharacterService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupMemberCharacterService.java:20 [EXTRACTED]
  ```
  public interface GroupMemberCharacterService {
  ```
- `GroupMemberService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupMemberService.java:16 [EXTRACTED]
  ```
  public interface GroupMemberService {
  ```
- `GroupService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupService.java:16 [EXTRACTED]
  ```
  public interface GroupService {
  ```
- `GroupTemplateService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/GroupTemplateService.java:14 [EXTRACTED]
  ```
  public interface GroupTemplateService {
  ```
- `JudgeService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/JudgeService.java:16 [EXTRACTED]
  ```
  public interface JudgeService {
  ```
- `PeriodScheduleService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PeriodScheduleService.java:16 [EXTRACTED]
  ```
  public interface PeriodScheduleService {
  ```
- `PersonBusinessService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PersonBusinessService.java:17 [EXTRACTED]
  ```
  public interface PersonBusinessService {
  ```
- `PersonIndicatorValueService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PersonIndicatorValueService.java:12 [EXTRACTED]
  ```
  public interface PersonIndicatorValueService {
  ```
- `PersonService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/exp/PersonService.java:14 [EXTRACTED]
  ```
  public interface PersonService {
  ```
- `RankListItemService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/rank/RankListItemService.java:17 [EXTRACTED]
  ```
  public interface RankListItemService {
  ```
- `RankListService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/rank/RankListService.java:19 [EXTRACTED]
  ```
  public interface RankListService {
  ```
- `ReportGroupService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/report/ReportGroupService.java:16 [EXTRACTED]
  ```
  public interface ReportGroupService {
  ```
- `ReportService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/service/report/ReportService.java:16 [EXTRACTED]
  ```
  public interface ReportService {
  ```
- `AigcConfigService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/aigc/AigcConfigService.java:16 [EXTRACTED]
  ```
  public interface AigcConfigService {
  ```
- `ArchiveService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/archive/ArchiveService.java:18 [EXTRACTED]
  ```
  public interface ArchiveService {
  ```
- `AssessService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/assess/AssessService.java:18 [EXTRACTED]
  ```
  public interface AssessService {
  ```
- `AdminAuthService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/auth/AdminAuthService.java:14 [EXTRACTED]
  ```
  public interface AdminAuthService {
  ```
- `BusinessBindService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessBindService.java:18 [EXTRACTED]
  ```
  public interface BusinessBindService {
  ```
- `BusinessInstitutionFileService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessInstitutionFileService.java:17 [EXTRACTED]
  ```
  public interface BusinessInstitutionFileService {
  ```
- `BusinessInstitutionQuestionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessInstitutionQuestionService.java:18 [EXTRACTED]
  ```
  public interface BusinessInstitutionQuestionService {
  ```
- `BusinessService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/business/BusinessService.java:19 [EXTRACTED]
  ```
  public interface BusinessService {
  ```
- `CaseArrangementService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseArrangementService.java:16 [EXTRACTED]
  ```
  public interface CaseArrangementService {
  ```
- `CaseBusinessFunctionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseBusinessFunctionService.java:19 [EXTRACTED]
  ```
  public interface CaseBusinessFunctionService {
  ```
- `CaseBusinessService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseBusinessService.java:19 [EXTRACTED]
  ```
  public interface CaseBusinessService {
  ```
- `CaseExperimentModeService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseExperimentModeService.java:6 [EXTRACTED]
  ```
  public interface CaseExperimentModeService {
  ```
- `CaseGridService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseGridService.java:16 [EXTRACTED]
  ```
  public interface CaseGridService {
  ```
- `CaseInfoService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseInfoService.java:18 [EXTRACTED]
  ```
  public interface CaseInfoService {
  ```
- `CaseInstitutionFileService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseInstitutionFileService.java:17 [EXTRACTED]
  ```
  public interface CaseInstitutionFileService {
  ```
- `CaseInstitutionQuestionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseInstitutionQuestionService.java:18 [EXTRACTED]
  ```
  public interface CaseInstitutionQuestionService {
  ```
- `CaseOrgService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseOrgService.java:15 [EXTRACTED]
  ```
  public interface CaseOrgService {
  ```
- `CaseSnapshotService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseSnapshotService.java:7 [EXTRACTED]
  ```
  public interface CaseSnapshotService {
  ```
- `CaseWeightService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/caseinfo/CaseWeightService.java:17 [EXTRACTED]
  ```
  public interface CaseWeightService {
  ```
- `CaseQuestionPreviewService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/casequestion/CaseQuestionPreviewService.java:16 [EXTRACTED]
  ```
  public interface CaseQuestionPreviewService {
  ```
- `CategoryService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/category/CategoryService.java:18 [EXTRACTED]
  ```
  public interface CategoryService {
  ```
- `CharacterService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/character/CharacterService.java:16 [EXTRACTED]
  ```
  public interface CharacterService {
  ```
- `ClazzService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/clazz/ClazzService.java:15 [EXTRACTED]
  ```
  public interface ClazzService {
  ```
- `CrwPlatformService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/crwplatform/CrwPlatformService.java:19 [EXTRACTED]
  ```
  public interface CrwPlatformService {
  ```
- `DeptService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dept/DeptService.java:16 [EXTRACTED]
  ```
  public interface DeptService {
  ```
- `PostService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dept/PostService.java:17 [EXTRACTED]
  ```
  public interface PostService {
  ```
- `DialogueMaterialService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dialoguematerial/DialogueMaterialService.java:16 [EXTRACTED]
  ```
  public interface DialogueMaterialService {
  ```
- `DialogueSynonymService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dialoguesynonym/DialogueSynonymService.java:8 [EXTRACTED]
  ```
  public interface DialogueSynonymService {
  ```
- `DictDataService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dict/DictDataService.java:17 [EXTRACTED]
  ```
  public interface DictDataService {
  ```
- `DictTypeService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/dict/DictTypeService.java:15 [EXTRACTED]
  ```
  public interface DictTypeService {
  ```
- `FileService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/file/FileService.java:18 [EXTRACTED]
  ```
  public interface FileService {
  ```
- `FunctionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/function/FunctionService.java:15 [EXTRACTED]
  ```
  public interface FunctionService {
  ```
- `IndicatorCategoryService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicator/IndicatorCategoryService.java:14 [EXTRACTED]
  ```
  public interface IndicatorCategoryService {
  ```
- `IndicatorService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicator/IndicatorService.java:18 [EXTRACTED]
  ```
  public interface IndicatorService {
  ```
- `CaseEvalIndicatorService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplate/CaseEvalIndicatorService.java:12 [EXTRACTED]
  ```
  public interface CaseEvalIndicatorService {
  ```
- `IndicatorTemplatePreviewService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplate/IndicatorTemplatePreviewService.java:12 [EXTRACTED]
  ```
  public interface IndicatorTemplatePreviewService {
  ```
- `IndicatorTemplateService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplate/IndicatorTemplateService.java:16 [EXTRACTED]
  ```
  public interface IndicatorTemplateService {
  ```
- `IndicatorTemplateCategoryService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplatecategory/IndicatorTemplateCategoryService.java:18 [EXTRACTED]
  ```
  public interface IndicatorTemplateCategoryService {
  ```
- `IndicatorTemplateIndicatorService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplateindicator/IndicatorTemplateIndicatorService.java:18 [EXTRACTED]
  ```
  public interface IndicatorTemplateIndicatorService {
  ```
- `IndicatorTemplateIndicatorWeightService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/indicatortemplateindicator/IndicatorTemplateIndicatorWeightService.java:13 [EXTRACTED]
  ```
  public interface IndicatorTemplateIndicatorWeightService {
  ```
- `InstitutionFileService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/institution/InstitutionFileService.java:14 [EXTRACTED]
  ```
  public interface InstitutionFileService {
  ```
- `InstitutionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/institution/InstitutionService.java:17 [EXTRACTED]
  ```
  public interface InstitutionService {
  ```
- `LoginLogService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/logger/LoginLogService.java:13 [EXTRACTED]
  ```
  public interface LoginLogService {
  ```
- `OperateLogService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/logger/OperateLogService.java:14 [EXTRACTED]
  ```
  public interface OperateLogService {
  ```
- `MailAccountService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailAccountService.java:17 [EXTRACTED]
  ```
  public interface MailAccountService {
  ```
- `MailLogService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailLogService.java:17 [EXTRACTED]
  ```
  public interface MailLogService {
  ```
- `MailSendService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailSendService.java:13 [EXTRACTED]
  ```
  public interface MailSendService {
  ```
- `MailTemplateService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/mail/MailTemplateService.java:18 [EXTRACTED]
  ```
  public interface MailTemplateService {
  ```
- `MemberService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/member/MemberService.java:8 [EXTRACTED]
  ```
  public interface MemberService {
  ```
- `NoticeService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notice/NoticeService.java:11 [EXTRACTED]
  ```
  public interface NoticeService {
  ```
- `NotifyMessageService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notify/NotifyMessageService.java:19 [EXTRACTED]
  ```
  public interface NotifyMessageService {
  ```
- `NotifySendService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notify/NotifySendService.java:11 [EXTRACTED]
  ```
  public interface NotifySendService {
  ```
- `NotifyTemplateService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/notify/NotifyTemplateService.java:16 [EXTRACTED]
  ```
  public interface NotifyTemplateService {
  ```
- `OAuth2ApproveService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2ApproveService.java:16 [EXTRACTED]
  ```
  public interface OAuth2ApproveService {
  ```
- `OAuth2ClientService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2ClientService.java:18 [EXTRACTED]
  ```
  public interface OAuth2ClientService {
  ```
- `OAuth2CodeService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2CodeService.java:14 [EXTRACTED]
  ```
  public interface OAuth2CodeService {
  ```
- `OAuth2GrantService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2GrantService.java:19 [EXTRACTED]
  ```
  public interface OAuth2GrantService {
  ```
- `OAuth2TokenService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/oauth2/OAuth2TokenService.java:16 [EXTRACTED]
  ```
  public interface OAuth2TokenService {
  ```
- `OperateService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/operate/OperateService.java:17 [EXTRACTED]
  ```
  public interface OperateService {
  ```
- `OrgService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/org/OrgService.java:16 [EXTRACTED]
  ```
  public interface OrgService {
  ```
- `MenuService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/MenuService.java:15 [EXTRACTED]
  ```
  public interface MenuService {
  ```
- `PermissionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/PermissionService.java:20 [EXTRACTED]
  ```
  public interface PermissionService {
  ```
- `RoleService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/permission/RoleService.java:20 [EXTRACTED]
  ```
  public interface RoleService {
  ```
- `PersonService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/person/PersonService.java:18 [EXTRACTED]
  ```
  public interface PersonService {
  ```
- `PersonDialogueMaterialService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/persondialoguematerial/PersonDialogueMaterialService.java:19 [EXTRACTED]
  ```
  public interface PersonDialogueMaterialService {
  ```
- `PersonIndicatorValueService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/personindicatorvalue/PersonIndicatorValueService.java:16 [EXTRACTED]
  ```
  public interface PersonIndicatorValueService {
  ```
- `FeedbackService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/portal/FeedbackService.java:16 [EXTRACTED]
  ```
  public interface FeedbackService {
  ```
- `PortalService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/portal/PortalService.java:19 [EXTRACTED]
  ```
  public interface PortalService {
  ```
- `TrialApplicationService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/portal/TrialApplicationService.java:16 [EXTRACTED]
  ```
  public interface TrialApplicationService {
  ```
- `ProdArrangementService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdArrangementService.java:16 [EXTRACTED]
  ```
  public interface ProdArrangementService {
  ```
- `ProdGridService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdGridService.java:16 [EXTRACTED]
  ```
  public interface ProdGridService {
  ```
- `ProdOrgService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdOrgService.java:12 [EXTRACTED]
  ```
  public interface ProdOrgService {
  ```
- `ProductService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProductService.java:17 [EXTRACTED]
  ```
  public interface ProductService {
  ```
- `ProdWeightService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/product/ProdWeightService.java:17 [EXTRACTED]
  ```
  public interface ProdWeightService {
  ```
- `QuestionOptionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/question/QuestionOptionService.java:14 [EXTRACTED]
  ```
  public interface QuestionOptionService {
  ```
- `QuestionService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/question/QuestionService.java:17 [EXTRACTED]
  ```
  public interface QuestionService {
  ```
- `SmsChannelService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsChannelService.java:18 [EXTRACTED]
  ```
  public interface SmsChannelService {
  ```
- `SmsCodeService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsCodeService.java:15 [EXTRACTED]
  ```
  public interface SmsCodeService {
  ```
- `SmsLogService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsLogService.java:17 [EXTRACTED]
  ```
  public interface SmsLogService {
  ```
- `SmsSendService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsSendService.java:13 [EXTRACTED]
  ```
  public interface SmsSendService {
  ```
- `SmsTemplateService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/sms/SmsTemplateService.java:17 [EXTRACTED]
  ```
  public interface SmsTemplateService {
  ```
- `SocialClientService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/social/SocialClientService.java:25 [EXTRACTED]
  ```
  public interface SocialClientService {
  ```
- `SocialUserService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/social/SocialUserService.java:19 [EXTRACTED]
  ```
  public interface SocialUserService {
  ```
- `TenantPackageService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantPackageService.java:16 [EXTRACTED]
  ```
  public interface TenantPackageService {
  ```
- `TenantService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenant/TenantService.java:21 [EXTRACTED]
  ```
  public interface TenantService {
  ```
- `TenantSyncSnapshotService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/tenantsyncsnapshot/TenantSyncSnapshotService.java:16 [EXTRACTED]
  ```
  public interface TenantSyncSnapshotService {
  ```
- `AdminUserService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/user/AdminUserService.java:27 [EXTRACTED]
  ```
  public interface AdminUserService {
  ```
- `UserClazzService` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/service/userclazz/UserClazzService.java:20 [EXTRACTED]
  ```
  public interface UserClazzService {
  ```
- `TenantFrameworkService` ← framework/eps-framework/eps-spring-boot-starter-biz-tenant/src/main/java/com/findsoft/education/framework/tenant/core/service/TenantFrameworkService.java:10 [EXTRACTED]
  ```
  public interface TenantFrameworkService {
  ```
- `SecurityFrameworkService` ← framework/eps-framework/eps-spring-boot-starter-security/src/main/java/com/findsoft/education/framework/security/core/service/SecurityFrameworkService.java:8 [EXTRACTED]
  ```
  public interface SecurityFrameworkService {
  ```
- `/infra/codegen` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:43 [EXTRACTED]
  ```
  @RequestMapping("/infra/codegen")
  ```
- `@Controller:CodegenController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:45 [EXTRACTED]
  ```
  public class CodegenController {
  ```
- `/db/table/list` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:50 [EXTRACTED]
  ```
  @GetMapping("/db/table/list")
  ```
- `/table/list` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:65 [EXTRACTED]
  ```
  @GetMapping("/table/list")
  ```
- `/table/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:74 [EXTRACTED]
  ```
  @GetMapping("/table/page")
  ```
- `/detail` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:82 [EXTRACTED]
  ```
  @GetMapping("/detail")
  ```
- `/create-list` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:94 [EXTRACTED]
  ```
  @PostMapping("/create-list")
  ```
- `/update` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:101 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/sync-from-db` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:109 [EXTRACTED]
  ```
  @PutMapping("/sync-from-db")
  ```
- `/delete` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:118 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/preview` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:127 [EXTRACTED]
  ```
  @GetMapping("/preview")
  ```
- `/download` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/codegen/CodegenController.java:136 [EXTRACTED]
  ```
  @GetMapping("/download")
  ```
- `/infra/config` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:34 [EXTRACTED]
  ```
  @RequestMapping("/infra/config")
  ```
- `@Controller:ConfigController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:36 [EXTRACTED]
  ```
  public class ConfigController {
  ```
- `/create` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:41 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:48 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:56 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:65 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:74 [EXTRACTED]
  ```
  @GetMapping(value = "/get")
  ```
- `/get-value-by-key` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:82 [EXTRACTED]
  ```
  @GetMapping(value = "/get-value-by-key")
  ```
- `/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:96 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/export` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/config/ConfigController.java:104 [EXTRACTED]
  ```
  @GetMapping("/export")
  ```
- `/infra/data-source-config` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:24 [EXTRACTED]
  ```
  @RequestMapping("/infra/data-source-config")
  ```
- `@Controller:DataSourceConfigController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:26 [EXTRACTED]
  ```
  public class DataSourceConfigController {
  ```
- `/create` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:31 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:38 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:46 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/get` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:55 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/list` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/db/DataSourceConfigController.java:64 [EXTRACTED]
  ```
  @GetMapping("/list")
  ```
- `/infra/file-config` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:25 [EXTRACTED]
  ```
  @RequestMapping("/infra/file-config")
  ```
- `@Controller:FileConfigController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:27 [EXTRACTED]
  ```
  public class FileConfigController {
  ```
- `/create` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:32 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:39 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/update-master` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:47 [EXTRACTED]
  ```
  @PutMapping("/update-master")
  ```
- `/delete` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:55 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/get` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:64 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:73 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/test` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileConfigController.java:81 [EXTRACTED]
  ```
  @GetMapping("/test")
  ```
- `/infra/file` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:36 [EXTRACTED]
  ```
  @RequestMapping("/infra/file")
  ```
- `@Controller:FileController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:39 [EXTRACTED]
  ```
  public class FileController {
  ```
- `/upload` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:44 [EXTRACTED]
  ```
  @PostMapping("/upload")
  ```
- `/domain` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:53 [EXTRACTED]
  ```
  @GetMapping("/domain")
  ```
- `/presigned-url` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:59 [EXTRACTED]
  ```
  @GetMapping("/presigned-url")
  ```
- `/create` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:71 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/delete` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:77 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/{configId}/get/**` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:86 [EXTRACTED]
  ```
  @GetMapping("/{configId}/get/**")
  ```
- `/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:112 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/compress` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/file/FileController.java:120 [EXTRACTED]
  ```
  @PostMapping("/compress")
  ```
- `/infra/job` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/job/JobController.java:16 [EXTRACTED]
  ```
  @RequestMapping("/infra/job")
  ```
- `@Controller:JobController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/job/JobController.java:18 [EXTRACTED]
  ```
  public class JobController {
  ```
- `/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/job/JobController.java:20 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/infra/api-access-log` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiAccessLogController.java:32 [EXTRACTED]
  ```
  @RequestMapping("/infra/api-access-log")
  ```
- `@Controller:ApiAccessLogController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiAccessLogController.java:34 [EXTRACTED]
  ```
  public class ApiAccessLogController {
  ```
- `/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiAccessLogController.java:39 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/export-excel` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiAccessLogController.java:47 [EXTRACTED]
  ```
  @GetMapping("/export-excel")
  ```
- `/infra/api-error-log` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java:33 [EXTRACTED]
  ```
  @RequestMapping("/infra/api-error-log")
  ```
- `@Controller:ApiErrorLogController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java:35 [EXTRACTED]
  ```
  public class ApiErrorLogController {
  ```
- `/update-status` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java:40 [EXTRACTED]
  ```
  @PutMapping("/update-status")
  ```
- `/page` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java:53 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/export-excel` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/logger/ApiErrorLogController.java:61 [EXTRACTED]
  ```
  @GetMapping("/export-excel")
  ```
- `/infra/redis` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/redis/RedisController.java:23 [EXTRACTED]
  ```
  @RequestMapping("/infra/redis")
  ```
- `@Controller:RedisController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/redis/RedisController.java:24 [EXTRACTED]
  ```
  public class RedisController {
  ```
- `/get-monitor-info` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/admin/redis/RedisController.java:29 [EXTRACTED]
  ```
  @GetMapping("/get-monitor-info")
  ```
- `/infra/file` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java:25 [EXTRACTED]
  ```
  @RequestMapping("/infra/file")
  ```
- `@Controller:AppFileController` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java:28 [EXTRACTED]
  ```
  public class AppFileController {
  ```
- `/upload` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java:33 [EXTRACTED]
  ```
  @PostMapping("/upload")
  ```
- `/presigned-url` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java:43 [EXTRACTED]
  ```
  @GetMapping("/presigned-url")
  ```
- `/create` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/controller/app/file/AppFileController.java:55 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `Demo01ContactService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/demo/demo01/Demo01ContactService.java:15 [EXTRACTED]
  ```
  public interface Demo01ContactService {
  ```
- `Demo02CategoryService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/demo/demo02/Demo02CategoryService.java:15 [EXTRACTED]
  ```
  public interface Demo02CategoryService {
  ```
- `Demo03StudentService` ← infra/eps-module-infra-server/src/main/java/com/findsoft/education/module/infra/service/demo/demo03/Demo03StudentService.java:19 [EXTRACTED]
  ```
  public interface Demo03StudentService {
  ```
- `/secman/case-snap` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:37 [EXTRACTED]
  ```
  @RequestMapping("/secman/case-snap")
  ```
- `@Controller:CaseSnapController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:39 [EXTRACTED]
  ```
  public class CaseSnapController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:44 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:51 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:59 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:68 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:77 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:86 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/export-excel` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/CaseSnapController.java:94 [EXTRACTED]
  ```
  @GetMapping("/export-excel")
  ```
- `/secman/experiment` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/secman/experiment")
  ```
- `@Controller:ExperimentController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:31 [EXTRACTED]
  ```
  public class ExperimentController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:36 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:43 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:51 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:60 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:69 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:78 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/uniform-start` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:86 [EXTRACTED]
  ```
  @PutMapping("/uniform-start")
  ```
- `/pause` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:95 [EXTRACTED]
  ```
  @PutMapping("/pause")
  ```
- `/resume` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/ExperimentController.java:104 [EXTRACTED]
  ```
  @PutMapping("/resume")
  ```
- `/secman/group` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/secman/group")
  ```
- `@Controller:GroupController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:31 [EXTRACTED]
  ```
  public class GroupController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:36 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:43 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:51 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:60 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:69 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupController.java:78 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/secman/group-member` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:26 [EXTRACTED]
  ```
  @RequestMapping("/secman/group-member")
  ```
- `@Controller:GroupMemberController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:28 [EXTRACTED]
  ```
  public class GroupMemberController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:33 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:40 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:48 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:57 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:66 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupMemberController.java:75 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/secman/group/template` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/secman/group/template")
  ```
- `@Controller:GroupTemplateController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:31 [EXTRACTED]
  ```
  public class GroupTemplateController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:36 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:43 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:51 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:60 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:69 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/GroupTemplateController.java:78 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/secman/judge` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:32 [EXTRACTED]
  ```
  @RequestMapping("/secman/judge")
  ```
- `@Controller:JudgeController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:34 [EXTRACTED]
  ```
  public class JudgeController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:39 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:46 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:54 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:63 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:72 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:81 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/export-excel` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/exp/JudgeController.java:89 [EXTRACTED]
  ```
  @GetMapping("/export-excel")
  ```
- `/secman/rank-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:35 [EXTRACTED]
  ```
  @RequestMapping("/secman/rank-list")
  ```
- `@Controller:RankListController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:37 [EXTRACTED]
  ```
  public class RankListController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:42 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:49 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:57 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:66 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:75 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:84 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/export-excel` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/rank/RankListController.java:92 [EXTRACTED]
  ```
  @GetMapping("/export-excel")
  ```
- `/secman/report` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:26 [EXTRACTED]
  ```
  @RequestMapping("/secman/report")
  ```
- `@Controller:ReportController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:28 [EXTRACTED]
  ```
  public class ReportController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:33 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:40 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:48 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:57 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:66 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportController.java:75 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/secman/report/group` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:26 [EXTRACTED]
  ```
  @RequestMapping("/secman/report/group")
  ```
- `@Controller:ReportGroupController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:28 [EXTRACTED]
  ```
  public class ReportGroupController {
  ```
- `/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:33 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:40 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:48 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:57 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:66 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/report/ReportGroupController.java:75 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/secman/crw-platform` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java:36 [EXTRACTED]
  ```
  @RequestMapping("/secman/crw-platform")
  ```
- `@Controller:CrwPlatformController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java:39 [EXTRACTED]
  ```
  public class CrwPlatformController {
  ```
- `/experiment/create` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java:49 [EXTRACTED]
  ```
  @PostMapping("/experiment/create")
  ```
- `/experiment/score/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java:55 [EXTRACTED]
  ```
  @GetMapping("/experiment/score/page")
  ```
- `/experiment/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/admin/thirdparty/CrwPlatformController.java:66 [EXTRACTED]
  ```
  @GetMapping("/experiment/page")
  ```
- `/secman/approval` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:24 [EXTRACTED]
  ```
  @RequestMapping("/secman/approval")
  ```
- `@Controller:AppApprovalController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:26 [EXTRACTED]
  ```
  public class AppApprovalController {
  ```
- `/submit` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:31 [EXTRACTED]
  ```
  @PostMapping("/submit")
  ```
- `/approve` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:45 [EXTRACTED]
  ```
  @PostMapping("/approve")
  ```
- `/reject` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:54 [EXTRACTED]
  ```
  @PostMapping("/reject")
  ```
- `/refuse` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:63 [EXTRACTED]
  ```
  @PostMapping("/refuse")
  ```
- `/detail` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:72 [EXTRACTED]
  ```
  @GetMapping("/detail")
  ```
- `/detail/{processId}` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:78 [EXTRACTED]
  ```
  @GetMapping("/detail/{processId}")
  ```
- `/pending-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:85 [EXTRACTED]
  ```
  @GetMapping("/pending-list")
  ```
- `/exp-record-list-by-experiment` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:91 [EXTRACTED]
  ```
  @GetMapping("/exp-record-list-by-experiment")
  ```
- `/exp-record-list-by-member` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:97 [EXTRACTED]
  ```
  @GetMapping("/exp-record-list-by-member")
  ```
- `/exp-record-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:103 [EXTRACTED]
  ```
  @GetMapping("/exp-record-list")
  ```
- `/exp-record-by-process` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/approval/AppApprovalController.java:110 [EXTRACTED]
  ```
  @GetMapping("/exp-record-by-process")
  ```
- `/secman/dialogue-record` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:36 [EXTRACTED]
  ```
  @RequestMapping("/secman/dialogue-record")
  ```
- `@Controller:DialogueRecordController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:38 [EXTRACTED]
  ```
  public class DialogueRecordController {
  ```
- `/ai-dialogue` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:43 [EXTRACTED]
  ```
  @PostMapping("/ai-dialogue")
  ```
- `/ai-dialogue-stream` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:51 [EXTRACTED]
  ```
  @PostMapping(value = "/ai-dialogue-stream", produces = MediaType.TEXT_EVENT_STREAM_VALUE)
  ```
- `/ai-dialogue-stop` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:98 [EXTRACTED]
  ```
  @PostMapping("/ai-dialogue-stop")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/dialoguerecord/DialogueRecordController.java:107 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/secman` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppEventController.java:25 [EXTRACTED]
  ```
  @RequestMapping("/secman")
  ```
- `@Controller:AppEventController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppEventController.java:27 [EXTRACTED]
  ```
  public class AppEventController {
  ```
- `/experiment/event/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppEventController.java:32 [EXTRACTED]
  ```
  @GetMapping("/experiment/event/get")
  ```
- `/secman/experiment/` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:31 [EXTRACTED]
  ```
  @RequestMapping("/secman/experiment/")
  ```
- `@Controller:AppExperimentController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:33 [EXTRACTED]
  ```
  public class AppExperimentController {
  ```
- `/dashboard` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:38 [EXTRACTED]
  ```
  @GetMapping("/dashboard")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:45 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:55 [EXTRACTED]
  ```
  @PostMapping("/page")
  ```
- `/my` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:66 [EXTRACTED]
  ```
  @GetMapping("/my")
  ```
- `/server-time` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentController.java:78 [EXTRACTED]
  ```
  @GetMapping("/server-time")
  ```
- `/secman/experiment/function` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:28 [EXTRACTED]
  ```
  @RequestMapping("/secman/experiment/function")
  ```
- `@Controller:AppExperimentFunctionController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:30 [EXTRACTED]
  ```
  public class AppExperimentFunctionController {
  ```
- `/list-business-functions` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:42 [EXTRACTED]
  ```
  @GetMapping("/list-business-functions")
  ```
- `/list-function-questions` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:54 [EXTRACTED]
  ```
  @GetMapping("/list-function-questions")
  ```
- `/get-function-person` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:67 [EXTRACTED]
  ```
  @GetMapping("/get-function-person")
  ```
- `/save-question` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:81 [EXTRACTED]
  ```
  @PostMapping("/save-question")
  ```
- `/institution/category-list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:90 [EXTRACTED]
  ```
  @GetMapping("/institution/category-list")
  ```
- `/list-institution-questions` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:106 [EXTRACTED]
  ```
  @GetMapping("/list-institution-questions")
  ```
- `/file/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentFunctionController.java:115 [EXTRACTED]
  ```
  @GetMapping("/file/page")
  ```
- `/secman/group` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:30 [EXTRACTED]
  ```
  @RequestMapping("/secman/group")
  ```
- `@Controller:AppExperimentGroupController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:32 [EXTRACTED]
  ```
  public class AppExperimentGroupController {
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:37 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:45 [EXTRACTED]
  ```
  @PostMapping("/page")
  ```
- `/rename` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:52 [EXTRACTED]
  ```
  @PutMapping("/rename")
  ```
- `/submit` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentGroupController.java:60 [EXTRACTED]
  ```
  @PutMapping("/submit")
  ```
- `/secman/indicator` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:31 [EXTRACTED]
  ```
  @RequestMapping("/secman/indicator")
  ```
- `@Controller:AppExperimentIndicatorController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:33 [EXTRACTED]
  ```
  public class AppExperimentIndicatorController {
  ```
- `/list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:40 [EXTRACTED]
  ```
  @GetMapping("/list")
  ```
- `/home` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:47 [EXTRACTED]
  ```
  @GetMapping("/home")
  ```
- `/group/current` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:55 [EXTRACTED]
  ```
  @GetMapping("/group/current")
  ```
- `/group/logs` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:63 [EXTRACTED]
  ```
  @GetMapping("/group/logs")
  ```
- `/group/limit` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:81 [EXTRACTED]
  ```
  @GetMapping("/group/limit")
  ```
- `/showOnSecondBoard` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentIndicatorController.java:91 [EXTRACTED]
  ```
  @GetMapping("/showOnSecondBoard")
  ```
- `/secman/member` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:28 [EXTRACTED]
  ```
  @RequestMapping("/secman/member")
  ```
- `@Controller:AppExperimentMemberController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:30 [EXTRACTED]
  ```
  public class AppExperimentMemberController {
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:35 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:43 [EXTRACTED]
  ```
  @PostMapping("/page")
  ```
- `/enter` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:53 [EXTRACTED]
  ```
  @PutMapping("/enter")
  ```
- `/leave` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentMemberController.java:64 [EXTRACTED]
  ```
  @PutMapping("/leave")
  ```
- `/secman/person` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java:27 [EXTRACTED]
  ```
  @RequestMapping("/secman/person")
  ```
- `@Controller:AppExperimentPersonController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java:29 [EXTRACTED]
  ```
  public class AppExperimentPersonController {
  ```
- `/top` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java:34 [EXTRACTED]
  ```
  @GetMapping("/top")
  ```
- `/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java:41 [EXTRACTED]
  ```
  @PostMapping("/page")
  ```
- `/get` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentPersonController.java:47 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/secman/experiment/rank/` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentRankListController.java:45 [EXTRACTED]
  ```
  @RequestMapping("/secman/experiment/rank/")
  ```
- `@Controller:AppExperimentRankListController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentRankListController.java:47 [EXTRACTED]
  ```
  public class AppExperimentRankListController {
  ```
- `/items/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentRankListController.java:52 [EXTRACTED]
  ```
  @GetMapping("/items/page")
  ```
- `/items/export-excel` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentRankListController.java:60 [EXTRACTED]
  ```
  @GetMapping("/items/export-excel")
  ```
- `/secman/experiment/score-test` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:37 [EXTRACTED]
  ```
  @RequestMapping("/secman/experiment/score-test")
  ```
- `@Controller:AppExperimentScoreTestController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:40 [EXTRACTED]
  ```
  public class AppExperimentScoreTestController {
  ```
- `/calculate-group` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:53 [EXTRACTED]
  ```
  @PostMapping("/calculate-group")
  ```
- `/calculate-total` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:73 [EXTRACTED]
  ```
  @PostMapping("/calculate-total")
  ```
- `/replay-check-answer` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:88 [EXTRACTED]
  ```
  @PostMapping("/replay-check-answer")
  ```
- `/update-group-indicator` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:100 [EXTRACTED]
  ```
  @PostMapping("/update-group-indicator")
  ```
- `/update-group-indicator-single` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:113 [EXTRACTED]
  ```
  @PostMapping("/update-group-indicator-single")
  ```
- `/send-mq` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppExperimentScoreTestController.java:132 [EXTRACTED]
  ```
  @PostMapping("/send-mq")
  ```
- `@Controller:AppGroupMemberCharacterController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppGroupMemberCharacterController.java:25 [EXTRACTED]
  ```
  public class AppGroupMemberCharacterController {
  ```
- `/secman/character/list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppGroupMemberCharacterController.java:31 [EXTRACTED]
  ```
  @GetMapping("/secman/character/list")
  ```
- `/secman/member/character/assign` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppGroupMemberCharacterController.java:38 [EXTRACTED]
  ```
  @PostMapping("/secman/member/character/assign")
  ```
- `/secman/member/character/list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppGroupMemberCharacterController.java:45 [EXTRACTED]
  ```
  @GetMapping("/secman/member/character/list")
  ```
- `/secman/orgs` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppOrgController.java:28 [EXTRACTED]
  ```
  @RequestMapping("/secman/orgs")
  ```
- `@Controller:AppOrgController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppOrgController.java:30 [EXTRACTED]
  ```
  public class AppOrgController {
  ```
- `/tree` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppOrgController.java:35 [EXTRACTED]
  ```
  @GetMapping("/tree")
  ```
- `/secman` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppPeriodNotificationController.java:27 [EXTRACTED]
  ```
  @RequestMapping("/secman")
  ```
- `@Controller:AppPeriodNotificationController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppPeriodNotificationController.java:29 [EXTRACTED]
  ```
  public class AppPeriodNotificationController {
  ```
- `/experiment/period/notification/list` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/exp/AppPeriodNotificationController.java:34 [EXTRACTED]
  ```
  @GetMapping("/experiment/period/notification/list")
  ```
- `/secman/report` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/report/AppReportController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/secman/report")
  ```
- `@Controller:AppReportController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/report/AppReportController.java:31 [EXTRACTED]
  ```
  public class AppReportController {
  ```
- `/preview-data` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/report/AppReportController.java:38 [EXTRACTED]
  ```
  @GetMapping("/preview-data")
  ```
- `/create-pdf` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/report/AppReportController.java:49 [EXTRACTED]
  ```
  @GetMapping("/create-pdf")
  ```
- `/secman/crw-platform` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/thirdparty/CrwPlatformAppController.java:36 [EXTRACTED]
  ```
  @RequestMapping("/secman/crw-platform")
  ```
- `@Controller:CrwPlatformAppController` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/thirdparty/CrwPlatformAppController.java:39 [EXTRACTED]
  ```
  public class CrwPlatformAppController {
  ```
- `/experiment/page` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/controller/app/thirdparty/CrwPlatformAppController.java:44 [EXTRACTED]
  ```
  @PostMapping("/experiment/page")
  ```
- `MqMessageService` ← secman-student/eps-secman-student-service-server/src/main/java/com/findsoft/education/module/secman/framework/mq/service/MqMessageService.java:8 [EXTRACTED]
  ```
  public interface MqMessageService {
  ```
- `/system/aigc-config` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/system/aigc-config")
  ```
- `@Controller:AigcConfigController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:31 [EXTRACTED]
  ```
  public class AigcConfigController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:38 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:45 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:53 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:62 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:71 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:80 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/test-connection` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/aigc/AigcConfigController.java:90 [EXTRACTED]
  ```
  @PostMapping("/test-connection")
  ```
- `/system/archive` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/system/archive")
  ```
- `@Controller:ArchiveController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:31 [EXTRACTED]
  ```
  public class ArchiveController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:36 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:43 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:51 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/batchDelete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:60 [EXTRACTED]
  ```
  @DeleteMapping("/batchDelete")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:69 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:78 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/preview` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/archive/ArchiveController.java:86 [EXTRACTED]
  ```
  @GetMapping("/preview")
  ```
- `/system/assess` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/system/assess")
  ```
- `@Controller:AssessController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:31 [EXTRACTED]
  ```
  public class AssessController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:36 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:43 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:51 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/batchDelete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:60 [EXTRACTED]
  ```
  @DeleteMapping("/batchDelete")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:69 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:78 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/preview` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/assess/AssessController.java:86 [EXTRACTED]
  ```
  @GetMapping("/preview")
  ```
- `/system/auth` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:65 [EXTRACTED]
  ```
  @RequestMapping("/system/auth")
  ```
- `@Controller:AuthController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:68 [EXTRACTED]
  ```
  public class AuthController {
  ```
- `/get-tenant-id-by-username` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:88 [EXTRACTED]
  ```
  @GetMapping("/get-tenant-id-by-username")
  ```
- `/login` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:101 [EXTRACTED]
  ```
  @PostMapping("/login")
  ```
- `/logout` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:108 [EXTRACTED]
  ```
  @PostMapping("/logout")
  ```
- `/refresh-token` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:120 [EXTRACTED]
  ```
  @PostMapping("/refresh-token")
  ```
- `/get-permission-info` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:128 [EXTRACTED]
  ```
  @GetMapping("/get-permission-info")
  ```
- `/register` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:154 [EXTRACTED]
  ```
  @PostMapping("/register")
  ```
- `/sms-login` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:163 [EXTRACTED]
  ```
  @PostMapping("/sms-login")
  ```
- `/send-sms-code` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:170 [EXTRACTED]
  ```
  @PostMapping("/send-sms-code")
  ```
- `/reset-password` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:178 [EXTRACTED]
  ```
  @PostMapping("/reset-password")
  ```
- `/social-auth-redirect` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:188 [EXTRACTED]
  ```
  @GetMapping("/social-auth-redirect")
  ```
- `/social-login` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/auth/AuthController.java:201 [EXTRACTED]
  ```
  @PostMapping("/social-login")
  ```
- `/system/business/bind` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:33 [EXTRACTED]
  ```
  @RequestMapping("/system/business/bind")
  ```
- `@Controller:BusinessBindController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:35 [EXTRACTED]
  ```
  public class BusinessBindController {
  ```
- `/create-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:43 [EXTRACTED]
  ```
  @PostMapping("/create-list")
  ```
- `/question/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:49 [EXTRACTED]
  ```
  @PostMapping("/question/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:56 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:64 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:73 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:82 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:91 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `/get-character-count` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessBindController.java:99 [EXTRACTED]
  ```
  @GetMapping("/get-character-count")
  ```
- `/system/business` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:31 [EXTRACTED]
  ```
  @RequestMapping("/system/business")
  ```
- `@Controller:BusinessController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:33 [EXTRACTED]
  ```
  public class BusinessController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:38 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:45 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:53 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:62 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:71 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:79 [EXTRACTED]
  ```
  @PostMapping("/page")
  ```
- `/copy` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessController.java:94 [EXTRACTED]
  ```
  @PostMapping("/copy")
  ```
- `/system/business/institution` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:36 [EXTRACTED]
  ```
  @RequestMapping("/system/business/institution")
  ```
- `@Controller:BusinessInstitutionController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:38 [EXTRACTED]
  ```
  public class BusinessInstitutionController {
  ```
- `/file/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:77 [EXTRACTED]
  ```
  @PostMapping("/file/create")
  ```
- `/file/create-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:84 [EXTRACTED]
  ```
  @PostMapping("/file/create-list")
  ```
- `/file/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:92 [EXTRACTED]
  ```
  @DeleteMapping("/file/delete")
  ```
- `/file/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:101 [EXTRACTED]
  ```
  @DeleteMapping("/file/delete-list")
  ```
- `/file/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:110 [EXTRACTED]
  ```
  @GetMapping("/file/get")
  ```
- `/file/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:119 [EXTRACTED]
  ```
  @GetMapping("/file/page")
  ```
- `/question/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:136 [EXTRACTED]
  ```
  @PostMapping("/question/create")
  ```
- `/question/create-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:143 [EXTRACTED]
  ```
  @PostMapping("/question/create-list")
  ```
- `/question/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:151 [EXTRACTED]
  ```
  @DeleteMapping("/question/delete")
  ```
- `/question/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:160 [EXTRACTED]
  ```
  @DeleteMapping("/question/delete-list")
  ```
- `/question/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:169 [EXTRACTED]
  ```
  @GetMapping("/question/get")
  ```
- `/question/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/business/BusinessInstitutionController.java:178 [EXTRACTED]
  ```
  @GetMapping("/question/page")
  ```
- `/system/captcha` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/captcha/CaptchaController.java:21 [EXTRACTED]
  ```
  @RequestMapping("/system/captcha")
  ```
- `@Controller:CaptchaController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/captcha/CaptchaController.java:22 [EXTRACTED]
  ```
  public class CaptchaController {
  ```
- `/check` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/captcha/CaptchaController.java:37 [EXTRACTED]
  ```
  @PostMapping("/check")
  ```
- `@Controller:CaseArrangementController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:33 [EXTRACTED]
  ```
  public class CaseArrangementController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:38 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:45 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:53 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:62 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:71 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseArrangementController.java:80 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `@Controller:CaseBusinessBindController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:34 [EXTRACTED]
  ```
  public class CaseBusinessBindController {
  ```
- `/bind/create-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:52 [EXTRACTED]
  ```
  @PostMapping("/bind/create-list")
  ```
- `/question/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:59 [EXTRACTED]
  ```
  @PostMapping("/question/create")
  ```
- `/operate/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:67 [EXTRACTED]
  ```
  @PostMapping("/operate/create")
  ```
- `/bind/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:75 [EXTRACTED]
  ```
  @PutMapping("/bind/update")
  ```
- `/bind/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:83 [EXTRACTED]
  ```
  @DeleteMapping("/bind/delete")
  ```
- `/bind/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:92 [EXTRACTED]
  ```
  @DeleteMapping("/bind/delete-list")
  ```
- `/bind/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:101 [EXTRACTED]
  ```
  @GetMapping("/bind/get")
  ```
- `/bind/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:110 [EXTRACTED]
  ```
  @GetMapping("/bind/page")
  ```
- `/bind/get-character-count` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessBindController.java:118 [EXTRACTED]
  ```
  @GetMapping("/bind/get-character-count")
  ```
- `/system/case/business/function` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:29 [EXTRACTED]
  ```
  @RequestMapping("/system/case/business/function")
  ```
- `@Controller:CaseBusinessFunctionController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:31 [EXTRACTED]
  ```
  public class CaseBusinessFunctionController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:36 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:43 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:51 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:60 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseBusinessFunctionController.java:69 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```
- `@Controller:CaseGridController` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:33 [EXTRACTED]
  ```
  public class CaseGridController {
  ```
- `/create` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:38 [EXTRACTED]
  ```
  @PostMapping("/create")
  ```
- `/update` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:45 [EXTRACTED]
  ```
  @PutMapping("/update")
  ```
- `/delete` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:53 [EXTRACTED]
  ```
  @DeleteMapping("/delete")
  ```
- `/delete-list` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:62 [EXTRACTED]
  ```
  @DeleteMapping("/delete-list")
  ```
- `/get` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:71 [EXTRACTED]
  ```
  @GetMapping("/get")
  ```
- `/page` ← system/eps-module-system-server/src/main/java/com/findsoft/education/module/system/controller/admin/caseinfo/CaseGridController.java:80 [EXTRACTED]
  ```
  @GetMapping("/page")
  ```