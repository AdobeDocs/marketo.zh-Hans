---
description: Salesforce诊断 — Marketo文档 — 产品文档
title: Salesforce诊断
exl-id: c449f938-9615-47cb-b232-613ec29068a3
source-git-commit: 15c3124a53ce55810b598c43e29e21321534c81f
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Salesforce诊断 {#salesforce-diagnostics}

我们的Salesforce集成的一部分包括Web应用程序中的Salesforce诊断页面。 此页面从失败的数据记录到Salesforce中捕获错误。 这些错误可能会有所帮助，但并不总是可读的。 因此，我们整理了一份备忘单，帮助解释错误消息。

## 访问诊断 {#access-diagnostics}

1. 单击齿轮图标并选择 **设置**.

   ![](assets/salesforce-diagnostics-1.png)

1. 在集成下，单击 **诊断**.

   ![](assets/salesforce-diagnostics-2.png)

## 错误备忘单 {#error-cheat-sheet}

**错误：** API_CURRENT_DISABLED\
**类别：** 访问/验证\
**消息：** 已为此用户禁用API\
**发生的情况：** 用户没有API访问权限\
**故障排除步骤：** Salesforce管理员需要授予用户API访问权限。

**错误：** AUTHENTICATION_FAIL\
**类别：** 身份验证\
**消息：** invalid_grant：身份验证失败\
**发生的情况：** 身份验证失败\
**故障排除步骤：** 断开与Salesforce的连接，然后重新连接。

**错误：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**类别：** 访问/验证\
**消息：** {&quot;errorCode&quot;：&quot;INVALID_SESSION_ID&quot;，&quot;message&quot;：&quot;会话过期或无效&quot;}\
**发生的情况：**

1 — 触发器代码导致更新失败。\
2 — 用户对给定对象没有对象级别的写入权限。

**故障排除步骤：**

1 — 查看失败的触发器。\
2 — 授予用户对对象的写入权限，或者禁用尝试写入对象的功能。

**错误：** CANNOT_UPDATE_CONVERSION_LEAD\
**类别：** 其他\
**消息：** 无法引用已转换的潜在客户\
**发生的情况：** 我们正在尝试在联系人和潜在客户的“最近活动记录”期间记录到已转换的潜在客户。 还看了几个这样的广告。\
**故障排除步骤：** 有关这方面的任何情况，请向我们的 [支持团队](https://nation.marketo.com/t5/Support/ct-p/Support).

**错误：** 实体_IS_LOCKED\
**类别：** 访问/验证\
**消息：** 实体已锁定以进行编辑\
**发生的情况：** 该记录处于审批流程中，在获得审批负责人的批准或拒绝之前，无法进行任何附加编辑。\
**故障排除步骤：** 请参阅上文。

**错误：** EXPIRES_ACCESS
**类别：** 身份验证
**消息：** invalid_grant：过期的访问/刷新令牌
**发生的情况：** 访问或刷新令牌已过期。 令牌的过期日期 [Salesforce中的会话设置](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**故障排除步骤：** 您需要重新进行身份验证。 断开Salesforce连接，然后重新连接。

**错误：** FAILED_WRITE\
**类别：** 间歇性\
**消息：** 已到达文件结尾\
**发生的情况：** Salesforce出现性能问题，可能是由于客户端的触发器性能缺佳所致。\
**故障排除步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作以解决有问题的触发器。

**错误：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**类别：** 访问/验证
**消息：** 因客户而异。
**发生的情况：** 对象的自定义验证规则失败。
**故障排除步骤：** 检查导致此错误的自定义验证规则。 由于这是自定义规则，因此必须一次性处理该错误。

**错误：** FIELD_FILTER_VALIDATION_EXCEPTION\
**类别：** 访问/验证\
**消息：** 值不存在或不匹配筛选条件\
**发生的情况：** 更新时强制执行Salesforce中现有的错误数据。\
**故障排除步骤：** 请参阅上文。

**错误：** FIELD_INTEGRITY_EXCEPTION\
**类别：** 访问/验证\
**消息：** 现有国家/地区不承认字段：省/市/自治区代码的状态值\
**发生的情况：** 更新时强制执行Salesforce中现有的错误数据。\
**故障排除步骤：** 请参阅上文。

**错误：** INACTIVE_ORGANIZATION\
**类别：** 身份验证\
**消息：** invalid_grant：不活动的组织\
**发生的情况：** 您的Salesforce组织不再处于活动状态。
**故障排除步骤：** 断开连接，然后从Salesforce重新连接。

**错误：** INACTIVE_USER
**类别：** 身份验证
**消息：** invalid_grant：非活动用户
**发生的情况：** Salesforce用户不再处于活动状态
**故障排除步骤：** 断开连接，然后从Salesforce重新连接。

**错误：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**类别：** 间歇性\
**消息：** （无其他消息）\
**发生的情况：** Salesforce实例处于维护模式。\
**故障排除步骤：** 等待系统维护完成，然后重试日志记录。

**错误：** UNFFECTED_ACCESS_ON_CROSS_REFERENCE_ENTITY
**类别：** 访问/验证
**消息：** 对象ID的访问权限不足
**发生的情况：** 无权访问任务的父记录。
**故障排除步骤：** 请参阅上文。

**错误：** UNFULSE_ACCESS_OR_READONLY\
**类别：** 访问/验证
**消息：** 对象ID的访问权限不足
**发生的情况：** “最近活动”日志记录无法编辑特定记录，因为用户没有写入权限。\
**故障排除步骤：** 在Salesforce中授予用户访问权限或禁用该用户对该对象的“最近活动”日志记录。

**错误：** INVALID_FIELD\
**类别：** 间歇性\
**消息：** Net：：ReadTimeout\
**发生的情况：** 请求超时。 这可能是由于交易速度太慢所致。\
**故障排除步骤：** 查看现有自定义项以了解延迟问题的可能原因，和/或禁用一个或所有对象的“最近活动日志记录”以减少负载。

**错误：** INVALID_FIELD_FOR_INSERT_UPDATE\
**类别：** 访问/验证\
**消息：** 无法创建/更新字段： MSE_Replied__c。请检查此字段的安全设置。
**发生的情况：** 用户不具有执行“最近活动”日志记录事务处理所需的“销售分析操作”自定义字段的写入权限。 团队可能已经安装了软件包，但尚未为用户启用正确的字段。\
**故障排除步骤：** Salesforce管理员需要授予对自定义字段的访问权限或关闭最近活动日志记录。

**错误：** INVALID_GRANT\
**类别：** 身份验证\
**消息：** invalid_grant： ip受限制\
**发生的情况：** 我们正在尝试访问您的Salesforce，但您的IP限制阻止我们执行此操作。\
**故障排除步骤：** 您的Salesforce管理员将需要允许列表我们的IP。 用户应联系支持人员以获取IP地址。

**错误：** 无效类型\
**类别：** 访问/验证\
**消息：** CreatedDate， （从任务中选择Id）来自潜在客户，其中Email=&#39;emailid&#39;^ERROR位于行:1:Column：53s不支持&#39;Lead&#39;对象类型。 如果您尝试使用自定义对象，请确保在实体名称后附加“__c”。 请引用您的WSDL或描述调用以获取适当的名称
**发生的情况：** 我们尝试从Salesforce查询用户无权访问的对象类型。 这很可能与用户无权访问Lead对象有关。\
**故障排除步骤：** 授予对Salesforce中Lead对象的读取和更新访问权限，或者关闭对Lead记录的电子邮件日志记录和最近活动日志记录。

**错误：** QUERY_TIMEOUT\
**类别：** 间歇性\
**消息：** 查询请求运行时间过长\
**发生的情况：** 请参阅上文。\
**故障排除步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作以解决有问题的触发器。

**错误：** REQUEST_LIMIT_EXCEEDED\
**类别：** 间歇性\
**消息：**
1 — 超出ConcurrentPerOrgLongTxn限制\
2 — 超出总请求数限制\
3 - ConcurrentRequest\
**发生的情况：**
1 — 超出并发请求限制，可能是由于触发代码效率低下。\
2 — 太多的集成使组织超过了24小时的滚动时段。\
**故障排除步骤：**
1 — 查看受影响对象上的现有触发器。 可能禁用一个或多个对象的汇总日志记录。\
2 — 从Salesforce购买更多API调用。 可能禁用一个或多个对象的汇总日志记录。

**错误：** REQUIRED_FIELD_MISSING\
**类别：** 访问/验证\
**消息：** 缺少必填字段： `[Amount_Committed_Private_Capital__c]`
**发生的情况：** 这通常发生在最近的活动日志记录中。 已将自定义字段设置为必填，但其中具有空值。 如果记录是使用自定义字段的空值创建的，然后设置为必需，则可能会发生这种情况。 当我们尝试更新记录时，即使我们未触及自定义字段，也必须满足相关要求。\
**故障排除步骤：** 手动更新缺少字段的值。 然后，您可以重试销售分析操作中的消息。

**错误：** 服务器不可用\
**类别：** 间歇性\
**消息：** 服务器太忙\
**发生的情况：** Salesforce出现性能问题，可能是由于客户的触发器未达到最佳状态\
**故障排除步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作，对有问题的触发器进行故障诊断。

**错误：** TXN_SECURITY_NO_ACCESS\
**类别：** 访问/验证\
**消息：** 由于组织中存在安全策略，不允许执行您请求的操作。 请联系您的管理员。**发生的情况：** 已设置某种安全限制 — 请参阅https://developer.salesforce.com/forums/?id=“记录ID”\
**故障排除步骤：** 请咨询您的Salesforce管理员，看看具体有什么限制。

**错误：** UNABLE_TO_LOCK_ROW\
**类别：** 间歇性\
**消息：** 无法获取此记录的独占访问权限或1条记录：“记录ID”\
**发生的情况：** 可能存在一个触发条件，导致多次尝试访问同一记录，在群组电子邮件中可能发生。\
**故障排除步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作以解决有问题的触发器。

**错误：** UNKNOWN_EXCEPTION
**类别：** 其他\
**消息：** 发生未知异常\
**发生的情况：** Salesforce中未经处理的异常。\
**故障排除步骤：** 用Salesforce提交一个案例，并复制错误消息中的数值。 这是Salesforce代码未正确处理错误。
