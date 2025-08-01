---
unique-page-id: 14745730
description: Salesforce诊断 — Marketo文档 — 产品文档
title: Salesforce诊断
exl-id: a2b5bd10-bc92-4fd4-bc1b-4e02b48c9d83
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1324'
ht-degree: 0%

---

# [!DNL Salesforce]诊断 {#salesforce-diagnostics}

我们的[!DNL Salesforce]集成的一部分包括Web应用程序中的[!DNL Salesforce]诊断页面。 此页面捕获到[!DNL Salesforce]的失败数据记录中的错误。 这些错误可能会有所帮助，但并不总是可读的。 因此，我们整理了一份备忘单来帮助解释错误消息。

**错误：** API_CURRENT_DISABLED
**类别：**&#x200B;访问/验证
**消息：**&#x200B;已对此用户禁用API
**发生的情况：**&#x200B;用户没有API访问权限
**疑难解答步骤：** [!DNL Salesforce]管理员需要授予用户API访问权限。

<br> 

**错误：** AUTHENTICATION_FAILED
**类别：**&#x200B;身份验证
**消息：** invalid_grant：身份验证失败
**发生的情况：**&#x200B;身份验证失败
**故障排除步骤：**&#x200B;断开与[!DNL Salesforce]的连接，然后重新连接。

<br> 

**错误：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY
**类别：**&#x200B;访问/验证
**消息：** {&quot;errorCode&quot;：&quot;INVALID_SESSION_ID&quot;，&quot;message&quot;：&quot;会话过期或无效&quot;}
**发生什么情况：**

1 — 触发器代码导致更新失败。
2 — 用户对给定对象没有对象级别的写入权限。

**疑难解答步骤：**

1 — 检查失败的触发器。
2 — 授予用户对对象的写入权限或禁用尝试写入对象的功能。

<br> 

**错误：** CANNOT_UPDATE_CONVERSION_LEAD
**类别：**&#x200B;其他
**消息：**&#x200B;无法引用已转换的潜在客户
**发生什么情况：**&#x200B;我们正在尝试在联系人和潜在客户的最近活动日志记录期间记录到已转换的潜在客户。 也看过几个这样的推介会。
**疑难解答步骤：**&#x200B;请向我们的[支持团队](https://nation.marketo.com/t5/Support/ct-p/Support)报告任何此类实例。

<br> 

**错误：** ENTITY_IS_LOKED
**类别：**&#x200B;访问/验证
**消息：**&#x200B;实体已锁定进行编辑
**发生的情况：**&#x200B;记录处于批准流程中，在获得拥有该批准的人批准或拒绝之前，该记录不会受到任何其他编辑。
**疑难解答步骤：**&#x200B;请参阅上文。

<br> 

**错误：** EXPIRED_ACCESS
**类别：**&#x200B;身份验证
**消息：** invalid_grant：访问/刷新令牌已过期
**发生的情况：**&#x200B;访问或刷新令牌已过期。 令牌将根据[ [!DNL Salesforce]中的](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)会话设置过期。
**疑难解答步骤：**&#x200B;您需要重新进行身份验证。 断开[!DNL Salesforce]连接并重新连接。

<br> 

**错误：** FAILED_WRITE
**类别：**&#x200B;间歇性
**消息：**&#x200B;已到达文件结尾
**发生什么情况：** [!DNL Salesforce]出现性能问题，可能是由于客户端的触发器性能缺佳。
**疑难解答步骤：**&#x200B;重试逻辑应处理此问题。 如果仍然不起作用，请与[!DNL Salesforce]管理员合作以解决有问题的触发器。

<br> 

**错误：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**类别：**&#x200B;访问/验证
**消息：**&#x200B;因客户而异。
**发生的情况：**&#x200B;对象的自定义验证规则失败。
**疑难解答步骤：**&#x200B;检查导致此错误的自定义验证规则。 由于这是自定义规则，因此必须一次性处理错误。

<br> 

**错误：** FIELD_FILTER_VALIDATION_EXCEPTION
**类别：**&#x200B;访问/验证
**消息：**&#x200B;值不存在或与筛选条件不匹配
**发生的情况：** [!DNL Salesforce]中的现有错误数据在更新时强制执行。
**疑难解答步骤：**&#x200B;请参阅上文。

<br> 

**错误：** FIELD_INTEGRITY_EXCEPTION
**类别：**&#x200B;访问/验证
**消息：**&#x200B;现有国家/地区不识别字段：州/省代码的状态值
**发生的情况：** [!DNL Salesforce]中的现有错误数据在更新时强制执行。
**疑难解答步骤：**&#x200B;请参阅上文。

<br> 

**错误：** INACTIVE_ORGANIZATION
**类别：**&#x200B;身份验证
**消息：** invalid_grant：不活动的组织
**发生的情况：**&#x200B;您的[!DNL Salesforce]组织不再处于活动状态。
**故障排除步骤：**&#x200B;断开连接，然后从[!DNL Salesforce]重新连接。

**错误：**&#x200B;非活动用户
**类别：**&#x200B;身份验证
**消息：** invalid_grant：非活动用户
**发生的情况：** [!DNL Salesforce]用户不再处于活动状态
**故障排除步骤：**&#x200B;断开连接，然后从[!DNL Salesforce]重新连接。

**错误：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE
**类别：**&#x200B;间歇性
**消息：** （无其他消息）
**发生的情况：** [!DNL Salesforce]实例处于维护模式。
**故障排除步骤：**&#x200B;等待系统维护完成，然后重试日志记录。

**错误：** UNEXPECTED_ACCESS_ON_CROSS_REFERENCE_ENTITY
**类别：**&#x200B;访问/验证
**消息：**&#x200B;对象ID访问权限不足
**发生的情况：**&#x200B;无法访问任务的父记录。
**疑难解答步骤：**&#x200B;请参阅上文。

<br> 

**错误：** INFIRMED_ACCESS_OR_READONLY
**类别：**&#x200B;访问/验证
**消息：**&#x200B;对象ID访问权限不足
**发生的情况：**&#x200B;最近活动日志记录无法编辑特定记录，因为用户没有写入权限。
**疑难解答步骤：**&#x200B;在[!DNL Salesforce]中授予用户访问权限或禁用该用户对该对象的最近活动日志记录。

**错误：** INVALID_FIELD
**类别：**&#x200B;间歇性
**消息：** Net：：ReadTimeout
**发生的情况：**&#x200B;请求超时。 这可能是由于事务过于缓慢所致。
**疑难解答步骤：**&#x200B;检查现有自定义项是否存在延迟问题的潜在原因，和/或禁用一个或多个对象的最新活动日志记录以减少负载。

**错误：** INVALID_FIELD_FOR_INSERT_UPDATE
**类别：**&#x200B;访问/验证
**消息：**&#x200B;无法创建/更新字段： ToutApp__Tout_Last_Replied__c。请检查此字段的安全设置。
**发生的情况：**&#x200B;用户没有执行最新活动日志记录事务所需的注销自定义字段的写入权限。 团队可能已经安装了软件包，但尚未为用户启用正确的字段。
**疑难解答步骤：** [!DNL Salesforce]管理员需要授予对自定义字段的访问权限或关闭最新活动日志记录。

**错误：** INVALID_GRANT
**类别：**&#x200B;身份验证
**消息：** invalid_grant： ip受限
**发生的情况：**&#x200B;我们正在尝试访问您的[!DNL Salesforce]，但您设置了IP限制阻止我们执行此操作。
**故障排除步骤：**&#x200B;您的[!DNL Salesforce]管理员需要允许列表我们的IP。 用户应联系支持人员以获取IP地址。

**错误：** INVALID_TYPE
**类别：**&#x200B;访问/验证
**消息：** CreatedDate， （从任务中选择ID） FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at `Row:1:Column:53sObject`不支持&#39;Lead&#39;类型。 如果您尝试使用自定义对象，请确保在实体名称后附加“__c”。 请参考您的WSDL或描述调用以获取适当的名称
**发生的情况：**&#x200B;我们正在尝试从Salesforce查询用户无权访问的对象类型。 这很可能与用户无权访问Lead对象有关。
**疑难解答步骤：**&#x200B;授予对Salesforce中Lead对象的读取和更新访问权限，或者关闭对Lead记录的电子邮件日志记录和最近活动日志记录。

**错误：** QUERY_TIMEOUT
**类别：**&#x200B;间歇性
**消息：**&#x200B;您的查询请求运行时间过长
**发生的情况：**&#x200B;请参阅上文。
**疑难解答步骤：**&#x200B;重试逻辑应处理此问题。 如果仍然不起作用，请与[!DNL Salesforce]管理员合作以解决触发器问题。

**错误：**&#x200B;已超出请求限制_EXCEEDED
**类别：**&#x200B;间歇性
**消息：**
1 — 超出ConcurrentPerOrgLongTxn限制
2 — 超出总请求数限制
3 - ConcurrentRequest
**发生什么情况：**
1 — 超出并发请求限制，可能是由于触发程序代码效率低下。
2 — 太多的集成使组织超过了24小时的滚动时段。
**疑难解答步骤：**
1 — 查看受影响对象上的现有触发器。 可能禁用一个或多个对象的汇总日志记录。
2 — 从[!DNL Salesforce]购买更多API调用。 可能禁用一个或多个对象的汇总日志记录。

**错误：** REQUIRED_FIELD_MISSING
**类别：**&#x200B;访问/验证
**消息：**&#x200B;缺少必填字段：`[Amount_Committed_Private_Capital__c]`
**发生的情况：**&#x200B;这通常发生在最近的活动日志记录中。 自定义字段已设置为必填，但其中具有空值。 如果记录是使用自定义字段的空值创建的，然后设置为必需，则可能会发生这种情况。 当我们尝试更新记录时，即使我们未触及自定义字段，也必须满足相关要求。
**疑难解答步骤：**&#x200B;手动更新缺少字段的值。 然后，您可以从ToutApp重试消息。

**错误：** SERVER_UNAVAILABLE
**类别：**&#x200B;间歇性
**邮件：**&#x200B;服务器太忙
**发生什么情况：**&#x200B;出现[!DNL Salesforce]性能问题，可能是由于客户触发的次优所致
**疑难解答步骤：**&#x200B;重试逻辑应处理此问题。 如果仍然不起作用，请与[!DNL Salesforce]管理员合作，对有问题的触发器进行故障诊断。

**错误：** TXN_SECURITY_NO_ACCESS
**类别：**&#x200B;访问/验证
**消息：**&#x200B;由于组织中存在安全策略，不允许执行您请求的操作。 请联系您的管理员。<br/>
**发生的情况：**&#x200B;已设置某种安全限制 — 请参阅https://developer.salesforce.com/forums/?id=“记录ID”
**疑难解答步骤：**&#x200B;与您的[!DNL Salesforce]管理员交谈，查看具体限制是什么。

**错误：** UNABLE_TO_LOCK_ROW
**类别：**&#x200B;间歇性
**消息：**&#x200B;无法独占访问此记录或1条记录：“记录ID”
**发生的情况：**&#x200B;可能有一个触发程序导致多次尝试访问同一记录，可能在群电子邮件中发生这种情况。
**疑难解答步骤：**&#x200B;重试逻辑应处理此问题。 如果仍然不起作用，请与[!DNL Salesforce]管理员合作以解决触发器问题。

**错误：** UNKNOWN_EXCEPTION
**类别：**&#x200B;其他
**消息：**&#x200B;发生未知异常
**发生的情况：**&#x200B;中出现[!DNL Salesforce]未处理的异常。
**疑难解答步骤：**&#x200B;将案例存档为[!DNL Salesforce]并复制错误消息中的数值。 这是[!DNL Salesforce]代码未正确处理错误。
