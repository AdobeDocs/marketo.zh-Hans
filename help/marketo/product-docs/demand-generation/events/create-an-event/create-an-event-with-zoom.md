---
unique-page-id: 17728023
description: 使用缩放创建事件 — Marketo文档 — 产品文档
title: 使用缩放创建事件
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
source-git-commit: 8b0625a7192a80986bc4295726cd13473493ddd7
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 使用缩放创建事件 {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [将缩放添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
* [创建新事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
* 设置相应的[流量操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以跟踪参与度


首先通过缩放创建网络研讨会。 Marketo会使用创建缩放时的某些设置，而某些设置则仅用于缩放。

在您创建Marketo活动并将缩放网络研讨会与之关联后，系统将能够共享注册和出席信息。 有关创建网络研讨会的帮助，请参阅[缩放网络研讨会快速入门](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)。

输入网络研讨会的以下信息，网络研讨会将通过适配器拉入Marketo。 如果您对此信息进行任何更改，则必须单击事件操作下方的“从网络研讨会提供程序刷新”链接，以便Marketo能够看到这些更改。

**标题和描述**

* **网络研讨会名称**  — 输入网络研讨会的名称。此名称将在Marketo中查看。

* **描述** （可选） — 输入网络研讨会的描述。描述将在Marketo中查看。

**日期和时间**

* **开始日期**  — 输入开始日期。该内容可在Marketo中查看。

* **开始时间**  — 输入开始时间。该内容可在Marketo中查看。

* **持续时间**  — 输入持续时间。开始时间和结束时间将在Marketo中查看。

* **时区**  — 选择适用的时区。该内容可在Marketo中查看。

* **定期网络研讨会** — 保持取消选中状态。

* **注册**  — 选中此框可进行注册。您将使用Marketo表单/登陆页面捕获将被推送到缩放的注册信息。

>[!NOTE]
Marketo当前不支持定期网络研讨会。 您必须在每个Marketo事件和缩放网络研讨会之间设置一个会话。

![](assets/overview2.png)

>[!TIP]
您将在缩放中配置其他字段，这些字段不会影响集成。 有关这些字段的其他信息，请参阅[缩放网络研讨会帮助中心](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar)。

现在，让我们跳进Marketo!

1. 选择一个事件。 单击&#x200B;**事件操作**&#x200B;并选择&#x200B;**事件设置**。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   所选事件的渠道类型必须是&#x200B;**网络研讨会**。

1. 从&#x200B;**Event** **Partner**&#x200B;列表中选择&#x200B;**Zoom**。

   ![](assets/eventsettings1.png)

1. 选择要将事件与关联的缩放帐户。

   ![](assets/selectaccount.png)

1. 选择网络研讨会。

   ![](assets/selectevent.png)

1. 单击&#x200B;**Save**。

   ![](assets/eventsettingssave.png)

   太棒了！ 现在，事件已通过缩放进行同步和计划。

   >[!NOTE]
   Marketo发送的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 确认URL发出后，此令牌会自动解析为人员的唯一确认URL。
   将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册且可能被取消订阅的用户仍会收到其确认信息。

   注册网络研讨会的人员将在“新状态”设置为“已注册”时，通过&#x200B;**更改项目状态**&#x200B;流程步骤推送到网络研讨会提供商。 没有其他状态会将人推过去。 另外，请务必执行&#x200B;**更改程序状态**&#x200B;流程步骤#1和&#x200B;**发送电子邮件**&#x200B;流程步骤#2。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   避免使用嵌套电子邮件程序发出确认电子邮件。 请改用事件项目的智能营销活动，如上所示。

   >[!TIP]
   数据可能最多需要48小时才能在Marketo中显示。 如果等待了那么长时间后仍未看到任何内容，请从事件&#x200B;**摘要**&#x200B;选项卡的“事件操作”菜单中选择&#x200B;**从网络研讨会提供程序刷新**。
