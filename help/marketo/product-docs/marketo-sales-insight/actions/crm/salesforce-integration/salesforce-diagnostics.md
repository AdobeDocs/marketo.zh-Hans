---
description: Salesforce诊断 — Marketo文档 — 产品文档
title: Salesforce诊断
exl-id: c449f938-9615-47cb-b232-613ec29068a3
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 0%

---

# Salesforce诊断 {#salesforce-diagnostics}

我们的Salesforce集成的一部分包括了Web应用程序中的Salesforce诊断页面。 此页面捕获无法将数据记录到Salesforce中产生的错误。 这些错误可能会有所帮助，但并不总是可读的。 因此，我们整理了一份备忘单来帮助解释错误消息。

## 访问诊断 {#access-diagnostics}

1. 单击齿轮图标，然后选择 **设置**.

   ![](assets/salesforce-diagnostics-1.png)

1. 在集成下，单击 **诊断**.

   ![](assets/salesforce-diagnostics-2.png)

## 错误备忘单 {#error-cheat-sheet}

**错误：** API_CURRENT_DISABLED\
**类别：** 访问/验证\
**消息：** 已为此用户禁用API\
**正在发生的情况：** 用户没有API访问权限\
**疑难解答步骤：** Salesforce管理员需要授予用户API访问权限。

**错误：** AUTHENTICATION_FAILED\
**类别：** 身份验证\
**消息：** invalid_grant：身份验证失败\
**正在发生的情况：** 身份验证失败\
**疑难解答步骤：** 断开与Salesforce的连接，然后重新连接。

**错误：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**类别：** 访问/验证\
**消息：** {&quot;errorCode&quot;：&quot;INVALID_SESSION_ID&quot;，&quot;message&quot;：&quot;会话过期或无效&quot;}\
**正在发生的情况：**

1 — 触发器代码导致更新失败。\
2 — 用户对给定对象没有对象级别的写入权限。

**疑难解答步骤：**

1 — 检查失败的触发器。\
2 — 授予用户对对象的写入权限或禁用尝试写入对象的功能。

**错误：** CANNOT_UPDATE_CONVERSION_LEAD\
**类别：** 其他\
**消息：** 无法引用已转换的潜在客户\
**正在发生的情况：** 我们正在尝试在“Contacts和Lead的最近活动记录”期间记录到已转化的Lead。 也看过几个这样的推介会。\
**疑难解答步骤：** 有关这方面的任何情况，请向我们的 [支持团队](https://nation.marketo.com/t5/Support/ct-p/Support).

**错误：** ENTITY_IS_LOCKING\
**类别：** 访问/验证\
**消息：** 实体已锁定以进行编辑\
**正在发生的情况：** 该记录处于审批流程中，在获得审批负责人的批准或拒绝之前，不会进行任何附加编辑。\
**疑难解答步骤：** 请参阅上文。

**错误：** EXPIRED_ACCESS
**类别：** 身份验证
**消息：** invalid_grant：过期的访问/刷新令牌
**正在发生的情况：** 访问或刷新令牌已过期。 令牌的过期日期 [Salesforce中的会话设置](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**疑难解答步骤：** 您需要重新进行身份验证。 断开Salesforce连接，然后重新连接。

**错误：** FAILED_WRITE\
**类别：** 间歇性\
**消息：** 已到达文件结尾\
**正在发生的情况：** Salesforce出现性能问题，可能是由于客户端的触发器性能缺佳所致。\
**疑难解答步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作，对有问题的触发器进行故障排除。

**错误：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**类别：** 访问/验证
**消息：** 因客户而异。
**正在发生的情况：** 对象的自定义验证规则失败。
**疑难解答步骤：** 检查导致此错误的自定义验证规则。 由于这是自定义规则，因此必须一次性处理错误。

**错误：** FIELD_FILTER_VALIDATION_EXCEPTION\
**类别：** 访问/验证\
**消息：** 值不存在或与筛选条件不匹配\
**正在发生的情况：** Salesforce中现有的错误数据在更新时强制执行。\
**疑难解答步骤：** 请参阅上文。

**错误：** FIELD_INTEGRITY_EXCEPTION\
**类别：** 访问/验证\
**消息：** 现有国家/地区不承认字段：省/市/自治区代码的状态值\
**正在发生的情况：** Salesforce中现有的错误数据在更新时强制执行。\
**疑难解答步骤：** 请参阅上文。

**错误：** INACTIVE_ORGANIZATION\
**类别：** 身份验证\
**消息：** invalid_grant：不活动的组织\
**正在发生的情况：** 您的Salesforce组织不再处于活动状态。
**疑难解答步骤：** 断开连接，然后重新与Salesforce连接。

**错误：** INACTIVE_USER
**类别：** 身份验证
**消息：** invalid_grant：非活动用户
**正在发生的情况：** Salesforce用户不再处于活动状态
**疑难解答步骤：** 断开连接，然后重新与Salesforce连接。

**错误：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**类别：** 间歇性\
**消息：** （无其他消息）\
**正在发生的情况：** Salesforce实例处于维护模式。\
**疑难解答步骤：** 等待系统维护完成，然后重试日志记录。

**错误：** UNFFECTED_ACCESS_ON_CROSS_REFERENCE_ENTITY
**类别：** 访问/验证
**消息：** 对象ID的访问权限不足
**正在发生的情况：** 无权访问任务的父记录。
**疑难解答步骤：** 请参阅上文。

**错误：** UNFFECTED_ACCESS_OR_READONLY\
**类别：** 访问/验证
**消息：** 对象ID的访问权限不足
**正在发生的情况：** 由于用户没有写入权限，因此最近活动日志记录无法编辑特定记录。\
**疑难解答步骤：** 在Salesforce中授予用户访问权限或为该用户禁用该对象的“最近活动”日志记录。

**错误：** INVALID_FIELD\
**类别：** 间歇性\
**消息：** Net：：ReadTimeout\
**正在发生的情况：** 请求超时。 这可能是由于事务过于缓慢所致。\
**疑难解答步骤：** 检查现有自定义项以了解延迟问题的潜在原因，和/或禁用一个或多个对象的“最近活动日志记录”以减少负载。

**错误：** INVALID_FIELD_FOR_INSERT_UPDATE\
**类别：** 访问/验证\
**消息：** 无法创建/更新字段： MSE_Replied__c。请检查此字段的安全设置。
**正在发生的情况：** 用户无权写入执行“最近活动日志记录”事务所需的“销售分析操作”自定义字段。 团队可能已经安装了软件包，但尚未为用户启用正确的字段。\
**疑难解答步骤：** Salesforce管理员需要授予对自定义字段的访问权限或关闭最近活动日志记录。

**错误：** INVALID_GRANT\
**类别：** 身份验证\
**消息：** invalid_grant： ip受限制\
**正在发生的情况：** 我们正在尝试访问您的Salesforce，但您实施了IP限制阻止我们执行此操作。\
**疑难解答步骤：** 您的Salesforce管理员将需要允许列表我们的IP。 用户应联系支持人员以获取IP地址。

**错误：** 无效类型\
**类别：** 访问/验证\
**消息：** CreatedDate， （从任务中选择ID）来自潜在客户，其中Email=&#39;emailid&#39;^ERROR位于行:1:Column：53sObject类型“潜在客户”不受支持。 如果您尝试使用自定义对象，请确保在实体名称后附加“__c”。 请参考您的WSDL或描述调用以获取适当的名称
**正在发生的情况：** 我们正在尝试从Salesforce查询用户无权访问的对象类型。 这很可能与用户无权访问Lead对象有关。\
**疑难解答步骤：** 授予对Salesforce中Lead对象的“读取”和“更新”访问权限，或者关闭对Lead记录的电子邮件日志记录和最近活动日志记录。

**错误：** QUERY_TIMEOUT\
**类别：** 间歇性\
**消息：** 您的查询请求运行时间过长\
**正在发生的情况：** 请参阅上文。\
**疑难解答步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作，对有问题的触发器进行故障排除。

**错误：** REQUEST_LIMIT_EXCEEDED\
**类别：** 间歇性\
**消息：**
1 — 超出ConcurrentPerOrgLongTxn限制\
2 — 超出总请求数限制\
3 - ConcurrentRequest\
**正在发生的情况：**
1 — 超出并发请求限制，可能是由于触发程序代码效率低下。\
2 — 太多的集成使组织超过了24小时的滚动时段。\
**疑难解答步骤：**
1 — 查看受影响对象上的现有触发器。 可能禁用一个或多个对象的汇总日志记录。\
2 — 从Salesforce购买更多API调用。 可能禁用一个或多个对象的汇总日志记录。

**错误：** REQUIRED_FIELD_MISSING\
**类别：** 访问/验证\
**消息：** 缺少必填字段： `[Amount_Committed_Private_Capital__c]`
**正在发生的情况：** 这通常发生在最近的活动日志记录中。 自定义字段已设置为必填，但其中具有空值。 如果记录是使用自定义字段的空值创建的，然后设置为必需，则可能会发生这种情况。 当我们尝试更新记录时，即使我们未触及自定义字段，也必须满足相关要求。\
**疑难解答步骤：** 手动更新缺少字段的值。 然后，您可以重试销售分析操作中的消息。

**错误：** 服务器不可用\
**类别：** 间歇性\
**消息：** 服务器太忙\
**正在发生的情况：** Salesforce出现性能问题，可能是由于客户触发的优化缺佳所致\
**疑难解答步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作，对有问题的触发器进行故障诊断。

**错误：** TXN_SECURITY_NO_ACCESS\
**类别：** 访问/验证\
**消息：** 由于组织中存在安全策略，不允许执行您请求的操作。 请联系您的管理员。**正在发生的情况：** 已设置某种安全限制 — 请参阅https://developer.salesforce.com/forums/?id=“记录ID”\
**疑难解答步骤：** 与Salesforce管理员交谈，了解具体限制是什么。

**错误：** UNABLE_TO_LOCK_ROW\
**类别：** 间歇性\
**消息：** 无法独占访问此记录或1条记录：“记录ID”\
**正在发生的情况：** 可能存在导致多次尝试访问同一记录的触发器，可能在群电子邮件的情况下。\
**疑难解答步骤：** 重试逻辑应处理此问题。 如果仍然不起作用，请与Salesforce管理员合作，对有问题的触发器进行故障排除。

**错误：** 未知异常
**类别：** 其他\
**消息：** 发生未知异常\
**正在发生的情况：** Salesforce中未经处理的异常。\
**疑难解答步骤：** 用Salesforce提交一个案例，并复制错误消息中的数值。 这是Salesforce代码未正确处理错误。
