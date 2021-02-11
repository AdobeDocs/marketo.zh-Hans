---
unique-page-id: 14745730
description: Salesforce诊断- Marketo文档——产品文档
title: Salesforce诊断
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---


# Salesforce诊断{#salesforce-diagnostics}

我们的Salesforce集成的一部分包括Web应用程序中的Salesforce诊断页面。 此页从失败的Salesforce数据记录中捕获错误。 这些错误可能有帮助，但并不总是可读。 因此，我们整理了一份备忘单，帮助解释错误信息。

**错误：** API_CURRENTLY_DISABLED\
**类别:** 访问／验证\
**消息：** 此用户已禁用API\
**正在发生** 的情况：用户没有API访问\
**疑难解答步** 骤：Salesforce管理员需要授予用户API访问权限。

<br> 

**错误：** AUTHENTICATION_FAILURE\
**类别：身** 份验证\
**消息：** invalid_grant:身份验证失败\
**正在发生什么：身份** 验证失败\
**疑难解答步骤：** 断开与Salesforce的连接，然后重新连接。

<br> 

**错误：** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**类别:** 访问／验证\
**消息** :{&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;会话已过期或无效&quot;}\
**正在发生的事情：**

1 —— 触发器代码导致更新失败。\
2 —— 用户对给定对象没有对象级写入权限。

**疑难解答步骤：**

1 —— 查看失败的触发器。\
2 —— 为对象授予用户写权限，或禁用尝试写入对象的功能。

<br> 

**错误：** CANNOT_UPDATE_CONVERTED_LEAD\
**类别：其** 他\
**消息：无** 法引用已转换的潜在客户\
**正在发生的事** 情：我们正在尝试在最近活动记录联系人和潜在客户期间登录已转换的潜在客户。还看过几个关于推销的。\
**疑难排解步** 骤：请向我们的支持团队报告此问题 [的任何实例](https://nation.marketo.com/t5/Support/ct-p/Support)。

<br> 

**错误：** ENTITY_IS_LOCKED\
**类别:** 访问／验证\
**消息：** 实体已锁定以进行编辑\
**正在发生的情** 况：该记录处于一个审批流程中，在获得审批人的批准或拒绝之前，该记录将被锁定，不进行任何其他编辑。\
**疑难解答步** 骤：请参阅上文。

<br> 

**错误：** EXPIRED_ACCESS
**类别** ：身份
**验证消** 息：invalid_grant:过期的访问／刷
**新令牌正在发** 生的情况：访问或刷新令牌已过期。令牌根据Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)中的[会话设置过期。
**疑难解答** 步骤：您需要重新验证。断开Salesforce连接并重新连接。

<br> 

**错误：** FAILED_WRITE\
**类别：间** 歇\
**消息：** 已到达文件结尾\
**正在发生的事** 情：Salesforce的性能问题，可能是由于客户端的次优触发器造成的。\
**疑难解答步骤：** 重试逻辑应处理此问题。如果它仍不工作，请与您的Salesforce管理员一起解决有问题的触发器。

<br> 

**错误：** FIELD_CUSTOM_VALIDATION_EXCEPTION
**类别:** 访问／验
**证消息：** 因客户而异。**正在发生的事** 情：对象的自定义验证规则失败。**疑难解答步** 骤：检查导致此错误的自定义验证规则。由于这是自定义规则，因此必须一次性处理错误。

<br> 

**错误：** FIELD_FILTER_VALIDATION_EXCEPTION\
**类别:** 访问／验证\
**消息：** 值不存在或与筛选条件不匹配\
**正在发生的情况：** Salesforce中现有的错误数据在更新后得到实施。\
**疑难解答步** 骤：请参阅上文。

<br> 

**错误：** FIELD_INTEGRITY_EXCEPTION\
**类别:** 访问／验证\
**消息：** 现有国家／地区不识别字段的状态值：州／省代码\
**正在发生的情况：** Salesforce中现有的错误数据在更新后得到实施。\
**疑难解答步** 骤：请参阅上文。

<br> 

**错误：** INACTIVE_ORGANIZATION\
**类别：身** 份验证\
**消息：** invalid_grant:非活动组织\
**发生的情况：** 您的Salesforce组织不再处于活动状态。\
**疑难解答步骤：** 断开连接，然后重新连接到Salesforce。

**错误：** INACTIVE_USER
**类别** ：身份
**验证消** 息：invalid_grant:非活动
**用户正在发生的** 事情：Salesforce用户不再是活动的疑难
**排解步骤：断** 开连接，然后重新连接到Salesforce。

**错误：** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**类别：间** 歇\
**消息：** （无其他消息）\
**正在发生的情况：** Salesforce实例处于维护模式。\
**疑难解答步骤：** 等到系统维护完成，然后重试日志记录。

**错误：** INFECIED_ACCESS_
**ON_CROSS_REFERENCE_ENTITY** 类别：访问／验证
**消息：对对象ID的访问权** 限不足正在发生的情况：
**** 任务无权访问父记录。**疑难解答步** 骤：请参阅上文。

<br> 

**错误：** INSUFICED_ACCESS_OR_READONLY\
**类别:** 访问／验
**证消息：对** 象id的访问权限不
**** 足正在发生的情况：最新活动记录无法编辑特定记录，因为用户没有写入访问权限。\
**疑难解答步骤：** 在Salesforce中授予用户访问权限，或为该用户禁用该对象的最新活动记录。

**错误：** INVALID_FIELD\
**类别：间** 歇\
**消息：** Net::ReadTimeout\
**正在发生的事** 情：请求是超时。这可能是交易太慢的结果。\
**疑难解答步** 骤：检查潜在延迟问题的罪魁祸首的现有自定义设置和／或为一个或多个对象禁用最新活动记录以减少负载。

**错误：** INVALID_FIELD_FOR_INSERT_UPDATE\
**类别:** 访问／验证\
**消息：** 无法创建／更新字段：ToutApp__Tout_Last_Rested__c。请检查此字段的安全设置。**正在发生的情** 况：用户没有写入权限访问执行“最近活动”日志记录事务所需的“输出”自定义字段。团队可能已安装包，但未为用户启用正确的字段。\
**疑难解答步** 骤：Salesforce管理员需要授予对自定义字段的访问权限或关闭最近活动记录。

**错误：** INVALID_GRANT\
**类别：身** 份验证\
**消息：** invalid_grant:受限\
**正在发生的情** 况：我们正在尝试访问您的Salesforce，但您已设置了IP限制，阻止我们访问。\
**疑难解答步** 骤：您的Salesforce管理员需要我允许列表们的IP。用户应联系支持部门以获取IP地址。

**错误：** INVALID_TYPE\
**类别:** 访问／验证\
**消息：** CreatedDate,(SELECT Id FROM任务)FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sObject type &#39;Lead&#39; is not supported.如果尝试使用自定义对象，请确保在实体名称后附加“__c”。 请引用WSDL或描述调用以获取相应的名称
**正在发生的情况：**&#x200B;我们正尝试从用户无权访问的Salesforce查询对象类型。 这很可能与用户无权访问潜在客户对象有关。\
**疑难解答步** 骤：向Salesforce中的潜在客户对象授予读取和更新访问权限，或关闭电子邮件记录和潜在客户记录的最近活动记录。

**错误：** 查询超时\
**类别：间** 歇\
**消息：** 您的查询请求运行时间过长\
**正在发生什么：** 请看上面。\
**疑难解答步骤：** 重试逻辑应处理此问题。如果它仍不工作，请与您的Salesforce管理员一起解决有问题的触发器。

**错误：** REQUEST_LIMIT_EXCEEDED\
**类别：间** 歇\
**消息：**
1 —— 超出ConcurrentPerOrgLongTxn限制\
2 —— 超出TotalRequests限制\
3 —— 并发请求\
**正在发生的情况：**
1 —— 超出并发请求限制，可能是由于触发代码效率低下所致。\
2 —— 过多集成使组织超过24小时滚动窗口。\
**疑难排解步**
骤：1 —— 查看受影响对象上的现有触发器。可能禁用一个或多个对象的汇总记录。\
2 —— 从Salesforce购买更多API调用。 可能禁用一个或多个对象的汇总记录。

**错误：** REQUIRED_FIELD_MISSING\
**类别:** 访问／验证\
**消息：** 必填字段缺失： `[Amount_Committed_Private_Capital__c]`
**正在发生的情况：** 这种情况通常发生在最新活动记录中。自定义字段设置为必填，但其值为空。 如果创建的记录具有自定义字段的空值，然后设置为必填，则会发生这种情况。 当我们尝试更新记录时，即使我们未触及自定义字段，也会强制执行要求。\
**疑难解答步** 骤：手动更新缺失字段的值。然后，您可以重试来自ToutApp的消息。

**错误：** SERVER_UNAVAILABLE\
**类别：间** 歇\
**消息：服** 务器太忙\
**发生的事情：** Salesforce的性能问题，可能由于客户的次优触发器\
**疑难解答步骤：** 重试逻辑应处理此问题。如果它仍不工作，请与您的Salesforce管理员合作，以便无法拍摄有问题的触发器。

**错误：** TXN_SECURITY_NO_ACCESS\
**类别:** 访问／验证\
**消息：** 由于您的组织中存在安全策略，因此不允许您请求的操作。与管理员联系。<br/>
**正在发生的** 情况：已设置某种安全限制——请参阅https://developer.salesforce.com/forums/?id=“记录ID”\
**疑难排解步** 骤：与Salesforce管理员交谈并查看具体限制是什么。

**错误：** UNABLE_TO_LOCK_ROW\
**类别：间** 歇\
**消息：** 无法获得对此记录或1记录的独占访问权限：&quot;记录ID&quot;\
**正在发生的** 事情：可能有一个触发器导致多次尝试访问同一记录，如果是群组电子邮件。\
**疑难解答步骤：** 重试逻辑应处理此问题。如果它仍不工作，请与您的Salesforce管理员一起解决有问题的触发器。

**错误：** UNKNOWN_EXCEPTION 
**类别:** 其他\
**消息：发** 生未知异常\
**正在发生的事** 件：Salesforce中未处理的异常。\
**疑难解答步** 骤：用Salesforce记录一个案例，并在错误消息中复制数字值。这是Salesforce代码无法正确处理错误。
