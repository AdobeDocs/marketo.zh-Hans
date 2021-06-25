---
unique-page-id: 2949874
description: 使用转到网络研讨会 — Marketo文档 — 产品文档创建事件
title: 使用GotoWebinar创建事件
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 使用GotoWebinar创建事件 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [将GoTo网络研讨会添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
* [创建新事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* 设置相应的[流量操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以跟踪参与度


首先在GoTo网络研讨会中创建网络研讨会。 创建GoTo网络研讨会中的某些设置由Marketo使用，而某些设置仅由GoTo网络研讨会使用。

在您创建Marketo活动并将GoTo网络研讨会与其关联后，系统将能够共享注册和出席信息。

以下是Marketo使用的设置列表。

## 标题和描述 {#title-and-description}

**网络研讨会名称**  — 输入网络研讨会的名称。此名称将在Marketo中查看。

**描述** （可选） — 输入网络研讨会的描述。描述将在Marketo中查看。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日期和时间 {#date-time}

输入网络研讨会的以下信息，网络研讨会将通过适配器拉入Marketo。 如果对此信息进行任何更改，必须单击&#x200B;**事件操作**&#x200B;下的链接“**从网络研讨会提供程序刷新**”，以便Marketo查看更改。

**开始日期**  — 输入开始日期。该内容可在Marketo中查看。

**开始时间**  — 输入开始时间。该内容可在Marketo中查看。

**结束时间**  — 输入结束时间。该内容可在Marketo中查看。

**时区**  — 选择适用的时区。可在Marketo中查看。

**类型 —** 设置为 **一个会话**。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
Marketo当前不支持定期网络研讨会。 您必须在每个Marketo活动与GoTo网络研讨会之间设置一个会话。

>[!TIP]
如果您需要其他GoTo网络研讨会帮助，请访问其[帮助网站](https://support.logmeininc.com/gotowebinar)。

现在，让我们跳进Marketo!

1. 选择一个事件。 单击&#x200B;**事件操作**&#x200B;并选择&#x200B;**事件设置**。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   所选事件的渠道类型必须是&#x200B;**网络研讨会**。

1. 从&#x200B;**事件合作伙伴**&#x200B;列表中选择&#x200B;**GoToWebinar**。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. 选择帐户。

   ![](assets/rtaimage-2.png)

1. 选择网络研讨会。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 单击&#x200B;**Save**。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 太棒了！ 现在，该事件由&#x200B;**GoToWebinar**&#x200B;同步和计划。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   Marketo发送的字段包括：名字、姓氏、电子邮件地址。 这些字段为必填字段，不得为空。

   >[!TIP]
   要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 确认URL发出后，此令牌会自动解析为人员的唯一确认URL。
   将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册且可能被取消订阅的用户仍会收到其确认信息。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   避免使用嵌套电子邮件程序发出确认电子邮件。 请改用事件项目的智能营销活动，如上所示。

   >[!TIP]
   数据可能最多需要48小时才能在Marketo中显示。 如果等待了那么长时间后仍未看到任何内容，请从事件&#x200B;**摘要**&#x200B;选项卡的“事件操作”菜单中选择&#x200B;**从网络研讨会提供程序刷新**。

注册网络研讨会的人员在将“新状态”设置为“已注册”时，将通过更改项目状态流程步骤推送到网络研讨会提供商。 没有其他状态会将人推过去。 另外，请务必执行更改项目状态流程步骤#1和发送电子邮件流程步骤#2。

## 查看计划  {#viewing-the-schedule}

在项目计划视图中，单击事件的日历条目。 您可以在屏幕右侧看到计划。

>[!NOTE]
要更改活动计划，您需要在GoTo网络研讨会上编辑网络研讨会。

![](assets/image2015-5-14-15-3a3-3a13.png)
