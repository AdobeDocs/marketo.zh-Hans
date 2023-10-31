---
description: 使用Webex创建事件 — Marketo文档 — 产品文档
title: 使用Webex创建事件
hide: true
hidefromtoc: true
feature: Events
source-git-commit: 286e1b7b563be70e932206adec6f80b4877b7953
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 使用Webex创建事件 {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [将Webex添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [创建新的事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的 [流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) 以跟踪参与情况

## 安排网络研讨会 {#schedule-a-webinar}

首先，在中创建网络研讨会 [Webex](https://www.webex.com/){target="_blank"}. Marketo Engage only uses specific settings and fields for your integration, which we'll go through shortly. For additional information, please see the [Webex Webinars Help Documentation](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

>[!NOTE]
>
>您可以在Webex中选择首选设置，但在Marketo Engage中只能查看以下信息：网络研讨会名称、开始/结束日期和时间、时区和描述。

### 基本信息 {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **主题**：这是您的事件名称，可在Marketo中查看。
* **日期和时间**：开始/结束日期、开始/结束时间、持续时间和时区都可以在Marketo中查看。
* **最大出席人数**：与会者的最大数量决定了支持的Webex功能。
* **与会者的网络广播视图**：选中此项以将您的网络研讨会实时流式传输到所有与会者。
* **座谈会成员**：邀请特定人员加入您的网络研讨会。
* **网络研讨会议程**：如果您要在发送给小组成员的电子邮件邀请中提供上下文，请填充此项。

### 安全性 {#security}

![](assets/create-an-event-with-webex-2.png)

* **网络研讨会密码**：（可选）如果您使用此字段，请确保将其包含在确认电子邮件中。
* **小组成员密码**：（可选）如果您使用此字段，请务必将其包含在您的网络研讨会议程中。
* **需要帐户**：将与会者限制为仅拥有Webex帐户的用户。

### 音频连接选项 {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **音频连接类型**：选择网络研讨会参与者如何加入网络研讨会的音频部分。
* **进入和退出色调**：选择当有人参加或退出网络研讨会时您希望用户听到的声音（需要电话音频连接）。
* **将小组成员静音**：选择所需的面板列表静音设置。

### 高级选项 {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **自动录制**：选中此项可自动录制网络研讨会。
* **实践会议**：选中此项可在网络研讨会开始时开始实践课程。
* **分组会话**：分组会话允许您在网络研讨会开始之前预先分配小组成员和与会者，或者允许您在网络研讨会期间加入。
* **网络研讨会系列**：将添加到网络研讨会系列可让人们查看您的网络研讨会，无论其是否公开。
* **注册**：要求与会者先注册并收到主机批准，然后才能参加。
* **电子邮件提醒**：选择网络研讨会开始前15分钟到两天内的电子邮件提醒。
* **网络研讨会选项**：确定哪些功能可供网络研讨会的参与者使用。
* **参与者权限**：参与者权限确定网络研讨会参与者可用的操作。

>[!NOTE]
>
>Marketo-Webex集成不支持从Webex发送确认电子邮件。 确认必须通过Marketo发送。 计划活动后，请确保将活动信息复制到Marketo确认电子邮件中，并将电子邮件设置为 _可操作_.

现在我们准备跳入Marketo Engage了！

## 将活动与Marketo Engage同步 {#sync-your-event-with-marketo-engage}

1. 在Marketo中，查找并选择您创建的事件程序。 在 **事件操作** 下拉列表，选择 **事件设置**.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >所选事件的渠道类型必须为 **网络研讨会**.

1. 在 **活动合作伙伴** 下拉列表，选择 **Webex网络研讨会**.

   ![](assets/create-an-event-with-webex-6.png)

1. 在 **登录** 从下拉菜单中选择您的Webex登录名。

   ![](assets/create-an-event-with-webex-7.png)

1. 在 **事件** 从下拉列表选择您的Webex事件。

   ![](assets/create-an-event-with-webex-8.png)

1. 将填充您的网络研讨会详细信息。 单击&#x200B;**保存**。

   ![](assets/create-an-event-with-webex-9.png)

您的Webex活动现在已与您的Marketo活动同步。 注册您的网络研讨会的用户将通过 _更改项目状态_ flow步骤。 没有其他状态会将该人员推倒。 请务必 _更改项目状态_ 流程步骤#1和 _发送电子邮件_ 流程步骤#2。

## 注意事项 {#things-to-note}

* 避免使用嵌套电子邮件程序发送确认电子邮件。 请改用事件程序的Smart Campaign。

* 数据可能需要48小时才能显示在Marketo中。 如果在等待了这么长时间后仍未看到任何内容，请单击 **从网络研讨会提供商刷新** 在 **事件操作** 中的下拉列表 **摘要** 选项卡。
