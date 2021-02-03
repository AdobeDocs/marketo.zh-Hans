---
unique-page-id: 17728023
description: 使用缩放——营销文档——产品文档创建事件
title: 使用缩放创建事件
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---


# 使用缩放{#create-an-event-with-zoom}创建事件

>[!PREREQUISITES]
>
>* [将缩放添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [创建新事件项目](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的[流动操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以跟踪参与情况


首先在缩放中创建网络研讨会。 Marketo会使用创建缩放时的某些设置，而某些设置仅由缩放使用。

创建Marketo事件并将缩放网络研讨会与其关联后，系统将能够共享注册和出席信息。 有关创建网络研讨会的帮助，请参阅[缩放网络研讨会入门](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar)。

为网络研讨会输入以下信息，该信息将通过适配器被引入Marketo。 如果您对此信息做了任何更改，则必须单击事件操作下的“从网络研讨会提供者刷新”链接，以便Market能够看到这些更改。

**标题和说明**

* **网络研讨会名称** -输入网络研讨会的名称。此名称将在Marketo中查看。

* **说明** （可选）-输入网络研讨会的说明。描述将可在Marketo中查看。

**日期和时间**

* **开始日** -输入开始日期。这将在Marketo中查看。

* **开始时间** -输入您的开始时间。这将在Marketo中查看。

* **持续时间** -输入持续时间。开始时间和结束时间将在Marketo中查看。

* **时区** -选择适用的时区。这将在Marketo中查看。

* **重复的网络研讨会**-保持未选中状态。

* **注册** -选中此框可进行注册。您将使用Marketo表单/登陆页来捕获将被推送到缩放的注册信息。

>[!NOTE]
>
>Marketo当前不支持重复的网络研讨会。 您必须在每个营销人员事件和缩放网络研讨会之间设置一个会话。

![](assets/overview2.png)

>[!TIP]
>
>您将在缩放中配置其他字段，这些字段不会影响集成。 有关这些字段的详细信息，请参阅[缩放网络研讨会帮助中心](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar)。

现在，让我们跳进市场！

1. 选择事件。 单击&#x200B;**事件操作**，然后选择&#x200B;**事件设置**。

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >所选渠道的事件类型必须为&#x200B;**网络研讨会**。

1. 从&#x200B;**事件****伙伴**&#x200B;列表选择&#x200B;**缩放**。

   ![](assets/eventsettings1.png)

1. 选择要与事件关联的缩放帐户。

   ![](assets/selectaccount.png)

1. 选择网络研讨会。

   ![](assets/selectevent.png)

1. 单击&#x200B;**保存**。

   ![](assets/eventsettingssave.png)

   太棒了！ 现在，事件已通过缩放进行同步和计划。

   >[!NOTE]
   >
   >Marketo发送到的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 发出确认URL时，此令牌会自动解析为个人的唯一确认URL。
   >
   >将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册并可能取消订阅的用户仍会收到其确认信息。

   注册网络研讨会的人员将通过&#x200B;**更改项目状态**&#x200B;流程步骤推送到网络研讨会提供者，当“新状态”设置为“已注册”时。 没有其他状态会把人推倒。 另外，请确保&#x200B;**更改项目状态**&#x200B;流步骤#1和&#x200B;**发送电子邮件**&#x200B;流步骤#2。

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件项目发送确认电子邮件。 请改用事件项目的智能活动，如上所示。

   >[!TIP]
   >
   >数据在Marketo中显示可能需要48小时。 如果等待那么长时间后仍看不到任何内容，请从事件的&#x200B;**摘要**&#x200B;选项卡的“事件操作”菜单中选择&#x200B;**从网络研讨会提供者**&#x200B;刷新。
