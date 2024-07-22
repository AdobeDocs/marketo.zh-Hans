---
unique-page-id: 2949863
description: 使用Webex创建事件 — Marketo文档 — 产品文档
title: 使用Webex创建事件
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 使用Webex创建事件 {#create-an-event-with-webex}

在Webex中创建网络研讨会后，您需要将活动与Marketo Engage同步。

>[!PREREQUISITES]
>
>* [将Webex添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [创建新的活动计划](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的[流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以跟踪参与

## 安排您的网络研讨会 {#schedule-your-webinar}

您可以在[Webex](https://www.webex.com/){target="_blank"}中计划活动并选择首选设置。 在Marketo中只能查看以下信息：网络研讨会名称、开始/结束日期和时间、时区和描述。 有关Webex网络研讨会[的其他信息可在此处](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}找到。

### 基本信息 {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **主题**：这是您的事件名称，可在Marketo中查看。
* **日期和时间**：“开始/结束日期”、“开始/结束时间”、“持续时间”和“时区”均可在Marketo中查看。
* **最大与会者数**：最大与会者数决定了支持哪些Webex功能。
* **与会者的网络广播视图**：选中此项可将您的网络研讨会实时流式传输到所有与会者。
* **座谈会成员**：邀请特定人员加入您的网络研讨会。
* **网络研讨会议程**：如果您要在发送给小组成员的电子邮件邀请中提供上下文，请填充此项。

### 安全性 {#security}

![](assets/create-an-event-with-webex-2.png)

* **网络研讨会密码**： （可选）如果您使用此字段，请务必将其包含在确认电子邮件中。
* **小组成员密码**： （可选）如果您使用此字段，请确保将其包含在网络研讨会议程中。
* **需要帐户**：将与会者限制为仅拥有Webex帐户的与会者。

### 音频连接选项 {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **音频连接类型**：选择网络研讨会参与者如何加入网络研讨会的音频部分。
* **进入和退出音调**：选择当有人进入或退出网络研讨会时您希望用户使用的音效（需要电话音频连接）。
* **将小组成员静音**：选择所需的小组成员静音设置。

### 高级选项 {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **自动录制**：选中此项以自动录制网络研讨会。
* **实践会议**：选中此项可在网络研讨会开始时启动实践会议。
* **分组会话**：分组会话允许您在网络研讨会开始之前预先分配小组成员和与会者，或者允许您在网络研讨会期间加入。
* **网络研讨会系列**：添加到网络研讨会系列可让用户查看您的网络研讨会，无论其是否公开。
* **注册**：要求与会者先注册并接收主机批准，然后才能参加。
* **电子邮件提醒**：选择网络研讨会开始前15分钟到2天的电子邮件提醒。
* **网络研讨会选项**：确定哪些功能可供网络研讨会中的参与者使用。
* **参与者权限**：参与者权限决定网络研讨会参与者可用的操作。

>[!NOTE]
>
>Marketo-Webex集成不支持从Webex发送确认电子邮件。 确认必须通过Marketo发送。 在安排活动后，请确保将活动信息复制到Marketo确认电子邮件并将电子邮件设置为&#x200B;_操作_。

## 将活动与Marketo Engage同步 {#sync-your-event-with-marketo-engage}

1. 在Marketo中，查找并选择所需的事件程序。 在&#x200B;**事件操作**&#x200B;下拉列表中，选择&#x200B;**事件设置**。

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >所选事件的渠道类型必须是&#x200B;**网络研讨会**。

1. 在&#x200B;**事件合作伙伴**&#x200B;下拉列表中，选择&#x200B;**Webex网络研讨会**。

   ![](assets/create-an-event-with-webex-6.png)

1. 在&#x200B;**登录**&#x200B;下拉列表中，选择您的Webex登录。

   ![](assets/create-an-event-with-webex-7.png)

1. 在&#x200B;**事件**&#x200B;下拉列表中，选择您的Webex事件。

   ![](assets/create-an-event-with-webex-8.png)

1. 将填充您的网络研讨会详细信息。 单击&#x200B;**保存**。

   ![](assets/create-an-event-with-webex-9.png)

您的Webex事件现在已与您的Marketo事件程序同步。 当新状态设置为“已注册”时，注册网络研讨会的用户将通过&#x200B;_更改计划状态_&#x200B;流程步骤推送至您的网络研讨会提供商。 没有其他状态会将该人员推倒。 请确保将&#x200B;_更改项目状态_&#x200B;流程步骤#1和&#x200B;_发送电子邮件_&#x200B;流程步骤#2。

## 注意事项 {#things-to-note}

* 避免使用嵌套电子邮件程序发送确认电子邮件。 请改用事件程序的Smart Campaign。

* 数据可能需要48小时才能显示在Marketo中。 如果等待了这么长时间，仍看不到任何内容，请单击事件程序&#x200B;**摘要**&#x200B;选项卡中&#x200B;**事件操作**&#x200B;下拉列表中的&#x200B;**从网络研讨会提供程序**&#x200B;刷新。
