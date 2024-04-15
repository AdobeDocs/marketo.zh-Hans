---
description: Dynamic Chat发行说明 — Marketo文档 — 产品文档
title: Dynamic Chat发行说明
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# 发行说明： 2024年4月 {#release-notes-apr-24}

Adobe Dynamic Chat版本在持续交付模型上运行，该模型允许采用更具可扩展性的方法来部署功能。 有时，一个月内会发布多个版本，因此请定期查看以获取最新信息。

用于Marketo Engage的标准发行说明页面 [可在此处找到](/help/marketo/release-notes/current.md){target="_blank"}.

## 4月版 {#april-release}

**发行日期： 2024年4月16日**

### 现在为Select包上的客户提供了对话流 {#conversational-flows-select-package}

当我们去年发布Conversational Flows时，Dynamic ChatSelect程序包上的客户只能利用此功能进行100次生命周期服务试用。 现在，对话流完全适用于Select包上的所有客户。

会话流程参与将计入Select程序包上客户每月最多参与250次的会话中。

### 回调函数 {#callback-functions}

回调函数允许您在访客与Dynamic Chat对话进行交互时，收集外部系统(如Adobe Analytics或Google Analytics)中的Dynamic Chat分析事件。 您可以通过在API中注册回调来侦听事件，从而启用Dynamic Chat分析事件。 这样，您就可以更全面地查看与其他关键数据（如Web流量）相关的Dynamic Chat参与情况。

### 向条件分支添加了实时代理可用性条件 {#live-agent-availability-conditional-branching}

除了本机字段和自定义Marketo字段之外，您现在还可以使用条件分支根据代理可用性创建分支。 如果您只想为访客提供在有实时代理可用时与实时代理通话的选项，则此功能非常有用。

屏幕快照

### 智能列表条件已添加到条件分支 {#smart-list-condition}

通过在条件分支中添加新的Marketo Engage智能列表条件，您可以根据已在Marketo中创建的预先存在的受众创建分支，而不是在Dynamic Chat中定义受众分支条件。

屏幕快照

### 对话流的条件分支 {#conditional-branching-for-conversational-flows}

今年早些时候，我们发布了对话的条件分支，现在您还可以利用对话流中的条件分支！ 条件分支允许您根据不同的条件在流中创建分支。

### 对话流的实时聊天 {#live-chat-for-conversational-flows}

我们去年发布了对话的实时聊天功能，现在您还可以将实时聊天参与添加到对话流程中。 如果您在Marketo表单中使用对话流程，您现在可以允许符合条件的访客在提交表单后立即与实时代理聊天！

### 代理收件箱中最近的Marketo Engage活动 {#recent-marketo-engage-activities-in-agent-inbox}

我们已将最近的Marketo Engage活动添加到代理收件箱的“最近的活动”部分，以便当网站访客请求与代理聊天时，代理可以轻松查看该访客最近是否参与了以下任何Marketo活动（最近25个活动）：

* 已打开的电子邮件
* 已访问网页
* 已填写表单
* 具有有趣的时刻

屏幕快照

### 代理管理中的日历连接状态 {#calendar-connection-status-in-agent-management}

管理员现在可以轻松查看哪些具有会议预订权限的座席已在Dynamic Chat中连接其日历。 这样，您就可以确保整个销售团队都已连接好，可以接受来自Dynamic Chat的会议邀请。

屏幕快照

### 代理日历配置中的最低通知设置 {#minimum-notice-setting-in-agent-calendar-configuration}

客户报告说，Web访客在其日历上预订会议时只收到十分钟的预告通知，因此我们在代理日历配置中引入了最低通知设置，并将默认提前期设置为24小时。

屏幕快照

### 新的应用程序内通知 {#new-in-app-notifications}

我们引入了三种新的应用程序内通知，帮助您实时了解Dynamic Chat实例的状态。

* 文本
* 文本
* 文本

### 添加/删除用户行为已更新 {#add-remove-user-behavior-updated}

有些客户告知我们他们在Dynamic Chat中添加和删除代理时遇到的问题，因此我们进行了一些更改以解决这些问题。

将用户添加到Live Chat或Meeting预订权限的Admin Console后，这些用户将立即显示在“代理管理”列表中，并可添加到对话框、对话流、路由规则和团队中。

从Admin Console中删除具有Meeting Booking或Live Chat权限的用户时，这些用户将立即从Dynamic Chat中删除，不再可用于Live Chat或Meeting路由，并且不再计入许可证限制。

### 改进了对话级别的报告性能 {#improved-conversation-level-report-performance}

现在，各个对话框和对话流量级别报表的性能更高、更准确。 以前，加载对话框报表可能需要几秒钟，并且数据有时与全局性能报表不一致。 现在，您的单个Dialogue报表将立即加载，并且数据将始终与全局报表数据保持一致。

屏幕快照

### 权限更新 {#permission-updates}

我们清理了Adobe Admin Console中的权限结构和命名，以使权限管理更直观。

* “对话管理”类别现在称为“对话”
* 会议类别现在称为活动
* “代理设置”类别现在称为“代理”
* “管理员设置”类别现在称为“配置”
* 实时聊天类别已删除，并且所有实时聊天权限已移至座席类别

屏幕快照

### 支持代理收件箱中的超链接 {#support-for-hyperlinks-in-agent-inbox}

现在，当实时聊天代理与聊天中的访客共享URL时，这些URL将超链接，以便访客只需单击它们即可导航到页面，而无需将URL复制并粘贴到浏览器中。

### 在代理收件箱中输入更新的密钥行为 {#enter-key-behavior-updated-in-agent-inbox}

我们切换了“代理收件箱”中的Return键行为，以便按Return或Enter键将发送您的消息，按Shift+Enter键将创建换行符。

屏幕快照

### 已删除循环调度页 {#round-robin-page-removed}

别担心！ 轮循路由仍然可以完全正常运行，并且运行方式与以往相同。 我们刚刚删除了显示代理及其在round robin路由队列中的顺序经常不准确的页面。

为了提供一些背景信息，当我们在2022年发布Dynamic Chat时，不支持live chat，仅设计了会议预约和循环路由页面，并专门考虑了会议预约。 随着去年实时聊天技术的推出，轮循页面已过时，因为它未准确反映具有会议预订和实时聊天权限的代理之间轮循路由的复杂性质。 我们探索了几种不同的方法来解决这个问题，但最终决定完全消除它是最大程度地减少混乱的最佳选择。

## 2月版 {#february-release}

**发行日期： 2024年2月22日**

### “对话”页面 {#conversations-page}

新的“对话”页面为您提供了一站式服务，可查看实例中发生的所有对话（自动和实时）的文字记录（来自已知和匿名潜在客户），让您更好地了解客户如何与您的对话、对话流程和实时代理进行互动。

屏幕快照

全局功能板中的日期范围从90天增加到24个月

你问，我们实现了。 现在，您可以在所有Analytics功能板中看到长达两年的Dynamic Chat参与数据。

### 对话框中的条件分支 {#conditional-branching-in-dialogues}

条件分支允许您根据不同的条件在Dialog流中创建分支。 现在，您可以根据Marketo中的商机和公司属性，在同一对话框中向不同人员展示不同的内容。

## 1月版 {#january-release}

**发行日期： 2024年1月24日**

### 代理管理中的并发实时聊天限制设置 {#Concurrent-live-chat-limit-setting}

默认情况下，您实例中的每个实时聊天代理一次最多可以参与5个实时聊天会话。 我们在代理管理中引入了新设置，通过该设置，您可以调整此限制（从1到10）。

屏幕快照
