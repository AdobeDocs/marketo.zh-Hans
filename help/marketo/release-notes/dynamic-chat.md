---
description: Dynamic Chat 发行说明 - Marketo Docs - 产品文档
title: Dynamic Chat发行说明
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 0015db05477cbb46a34e8abd4800d00c6522496f
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# Dynamic Chat发行说明 {#dynamic-chat-release}

Adobe Dynamic Chat版本在持续交付模型上运行，该模型允许采用更具可扩展性的方法来部署功能。 有时，一个月内会发布多个版本，因此请定期查看以获取最新信息。

可以在此处](/help/marketo/release-notes/current.md){target="_blank"}找到Marketo Engage[的标准发行说明页面。

## 2024年6月版 {#june-release}

**发行日期： 2024年6月6日**

### 对话流卡 {#conversational-flow-card}

利用对话流卡简化对话框中流中的多个步骤。

示例：如果您的目标是通过多个对话框推动网络研讨会的注册，则必须在所有具有该目标的对话框中重新创建相同的流程。 如果您必须更新任何详细信息，则必须逐个编辑每个对话框。 现在情况已发生了变化，这要归功于“对话流”卡。

除了跨多个对话框重新调整流用途之外，您还可以使用相同的过渡流触发其他渠道，如表单和登陆页面。

![](assets/dynamic-chat-june-2024-release-1.png)

### 使用限制 {#usage-limits}

“使用限制”页面会显示重要信息，例如包详细信息和使用限制状态。

![](assets/dynamic-chat-june-2024-release-2.png)

## 2024年5月版 {#may-release}

**发行日期： 2024年5月15日**

### 预批准的响应库 {#pre-approved-response-library}

[创建营销批准的库](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} AI生成的问题和答案，以帮助在几分钟内设置创作AI聊天。

![](assets/dynamic-chat-may-2024-release-1.png)

### 未解答的问题 {#unanswered-questions}

[使用以前对话中未回答问题的存储库](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"}生成新的预批准响应，并维护包含最新信息的响应库。

![](assets/dynamic-chat-may-2024-release-2.png)

### 对话摘要 {#conversation-summaries}

[为销售代理提供总结的对话](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"}，包括会议前对关键讨论主题的深入分析，以缩短准备时间，更好地为销售代理提供最新信息。

![](assets/dynamic-chat-may-2024-release-3.png)

### GenAI销售快捷方式 {#genai-sales-shortcuts}

[以更快的方式提供实时聊天代理](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"}以访问AI生成的响应、编辑现有生成的响应并搜索要在对话期间发送给购买者的其他内容。

![](assets/dynamic-chat-may-2024-release-4.png)

### 对话助手 {#conversation-assist}

使用您的营销团队预批准的响应，帮助销售代理在实时对话中做出准确响应。

### 对话轻推 {#conversation-nudges}

通过行动号召来推动Web访客，以促使对话结束。

<p>

## 2024年4月版 {#april-release}

**发行日期： 2024年4月23日**

### 对话流现在可供所有用户使用 {#conversational-flows-available-to-all-users}

允许符合条件的潜在客户在提交表单后立即通过Conversational Forms预约会议或与Sales聊天，从而使您的表单和登陆页更具对话性并缩短销售漏斗。现在，所有Dynamic Chat用户均可完全使用&#42;。

_&#42;以前作为试用功能提供，有100个生命周期参与。 会话流参与现在将计入Select包上用户250次参与会话的每月限制。_

### 回调函数 {#callback-functions}

[回调函数](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"}允许您在外部系统(如Adobe Analytics或Google Analytics)中收集Dynamic Chat分析事件，因为访客将参与Dynamic Chat对话。 您可以通过在API中注册回调来侦听事件，从而启用Dynamic Chat分析事件。 这样，您就可以更全面地了解Dynamic Chat参与情况，因为它与其他关键数据（如Web流量）相关。

### 向条件分支添加了实时代理可用性条件 {#live-agent-availability-conditional-branching}

除了本地和自定义Marketo Engage字段外，您现在还可以使用条件分支根据代理可用性创建分支。 如果您只想为访客提供在有实时代理可用时与实时代理通话的选项，则此功能非常有用。

![](assets/dynamic-chat-release-1.png)

### 智能列表条件已添加到条件分支 {#smart-list-condition}

通过在条件分支中添加新的Marketo Engage智能列表条件，您可以根据已在Marketo Engage中创建的预先存在的受众创建分支，而不是在Dynamic Chat中定义受众分支条件。

![](assets/dynamic-chat-release-2.png)

### 对话流的条件分支 {#conditional-branching-for-conversational-flows}

今年早些时候，我们发布了对话的条件分支，现在您还可以利用对话流中的条件分支！ 条件分支允许您根据不同的条件在流中创建分支。

### 对话流的实时聊天 {#live-chat-for-conversational-flows}

我们在2023年发布了对话的实时聊天功能，现在您还可以将实时聊天参与添加到对话流程中。 如果您在Marketo Engage表单中使用对话流程，您现在可以允许符合条件的访客在表单提交后立即与实时代理聊天！

### 代理收件箱中最近的Marketo Engage活动 {#recent-marketo-engage-activities-in-agent-inbox}

我们已将最近的Marketo Engage活动添加到代理收件箱的“最近的活动”部分，因此当网站访客请求与代理聊天时，代理可以快速查看该访客最近是否参与了以下任何Marketo Engage活动（最近25个活动）：

* 已打开的电子邮件
* 已访问网页
* 已填写表单
* 具有有趣的时刻

![](assets/dynamic-chat-release-3.png)

### 代理管理中的日历连接状态 {#calendar-connection-status-in-agent-management}

管理员现在可以轻松查看哪些具有会议预订权限的座席已在Dynamic Chat中连接其日历。 这样，您就可以确保整个Dynamic Chat团队都已连接并准备好接受销售人员的会议邀请。

![](assets/dynamic-chat-release-4.png)

### 代理日历配置中的最低通知设置 {#minimum-notice-setting-in-agent-calendar-configuration}

用户报告说，Web访客在其日历中预订会议，只需提前10分钟通知，因此我们在代理日历配置中引入了最低通知设置，并将默认提前期设置为24小时。

![](assets/dynamic-chat-release-5.png)

### 添加/删除用户行为已更新 {#add-remove-user-behavior-updated}

一些用户表示在Dynamic Chat中添加和删除代理时出现问题，因此我们进行了一些更改以解决这些问题。

将用户添加到Live Chat或Meeting预订权限的Admin Console后，这些用户将立即显示在“代理管理”列表中，并可添加到对话框、对话流、路由规则和团队中。

从Admin Console中删除具有Meeting Booking或Live Chat权限的用户时，这些用户将立即从Dynamic Chat中删除，不再可用于Live Chat或Meeting路由，并且不再计入许可证限制。

### 改进了对话级别的报告性能 {#improved-conversation-level-report-performance}

现在，各个对话框和对话流量级别报表的性能更高、更准确。 以前，加载对话框报表可能需要几秒钟时间，并且数据有时与全局性能报表不一致。 现在，您的单个对话框报表会立即加载，并且数据将始终与全局报表数据保持一致。

![](assets/dynamic-chat-release-6.png)

### 权限更新 {#permission-updates}

我们清理了Adobe Admin Console中的权限结构和命名，以使权限管理更直观。

* “对话管理”类别现在称为“对话”
* “会议”类别现在称为“活动”
* “代理设置”类别现在称为“代理”
* “管理员设置”类别现在称为“配置”
* 已删除“实时聊天”类别，并且所有实时聊天权限均已移至“座席”类别

![](assets/dynamic-chat-release-7.png)

### 支持代理收件箱中的超链接 {#support-for-hyperlinks-in-agent-inbox}

现在，当实时聊天代理与聊天中的访客共享URL时，这些URL将超链接，因此访客只需单击它们即可导航到页面，而无需将URL复制并粘贴到浏览器中。

### 在代理收件箱中输入更新的密钥行为 {#enter-key-behavior-updated-in-agent-inbox}

我们切换了“代理收件箱”中的返回键行为，因此按Return或Enter键将发送您的消息，按Shift+Enter将创建换行符。

![](assets/dynamic-chat-release-8.png)

### 已删除循环调度页 {#round-robin-page-removed}

别担心！ 轮循路由仍然可以完全正常运行，并且运行方式与以往相同。 我们刚刚删除了显示代理及其在round robin路由队列中的顺序经常不准确的页面。

2022年，我们发布Dynamic Chat时，不支持live chat，只支持会议预订，并且设计了循环路由页面，其中只考虑会议预订。 随着去年实时聊天技术的推出，轮循页面已过时，因为它未能准确反映具有会议预订和实时聊天权限的代理之间轮循路由的复杂性质。 我们探索了几种不同的方法来解决这个问题，但最终决定完全消除它是最大程度地减少混乱的最佳选择。

![](assets/dynamic-chat-release-9.png)

## 2024年2月版 {#february-release}

**发行日期： 2024年2月22日**

### “对话”页面 {#conversations-page}

新的“对话”页面为您提供了一站式服务，可查看实例中发生的所有对话（自动化和实时）的文字记录（来自已知和匿名潜在客户），让您更好地了解客户如何与您的对话、对话流程和实时代理进行互动。

![](assets/dynamic-chat-release-10.png)

### 全局功能板中的日期范围从90天增加到24个月 {#date-range-in-global-dashboard}

你问，我们实现了。 现在，您可以在所有Analytics功能板中看到长达两年的Dynamic Chat参与数据。

### 对话框中的条件分支 {#conditional-branching-in-dialogues}

条件分支允许您根据不同的条件在Dialog流中创建分支。 现在，您可以根据Marketo Engage中的商机和公司属性，在同一对话框中向不同人员展示不同的内容。

## 2024年1月版 {#january-release}

**发行日期： 2024年1月24日**

### 代理管理中的并发实时聊天限制设置 {#Concurrent-live-chat-limit-setting}

默认情况下，您实例中的每个实时聊天代理一次最多可以参与5个实时聊天会话。 我们在代理管理中引入了新设置，允许您将此限制从1调整为10。

![](assets/dynamic-chat-release-11.png)
