---
unique-page-id: 2949865
description: 使用Adobe Connect创建事件 — Marketo文档 — 产品文档
title: 使用Adobe Connect创建活动
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# 使用Adobe Connect创建活动 {#create-an-event-with-adobe-connect}

与Adobe Connect同步允许您管理Marketo中的网络研讨会注册和出席情况，这可以确保参与情况不会被取消跟踪。

>[!PREREQUISITES]
>
>* [链接Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [创建新的活动计划](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

首先，确保您已在Adobe Connect中创建了会议或研讨会。 如果您需要帮助，请查看[Adobe Connect用户指南](https://help.adobe.com/en_US/connect/9.0/using/index.html)。

您在Adobe Connect中创建的会议和研讨会必须在您在Marketo中输入凭据时指定的文件夹下创建。 创建会议或研讨会后，记下任何相关的后勤信息（如电话号码），以便在确认电子邮件和ICS文件中使用。

>[!CAUTION]
>
>作为活动主持人，请确保从应用程序内加入，并且&#x200B;**不能通过发送给与会者的链接加入**。

>[!NOTE]
>
>我们目前不支持现场Adobe Connect。

1. 在新事件的主页上，选择&#x200B;**[!UICONTROL Event Actions]**，然后选择&#x200B;**[!UICONTROL Event Settings]**。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果您在下拉列表中未看到&#x200B;**[!UICONTROL Event Settings]**，请确保该事件的渠道已在“**[!UICONTROL Event with Webinar]**”下选择[!UICONTROL Applies to]。

1. 在&#x200B;**[!UICONTROL Event Partner]**&#x200B;下，选择&#x200B;**[!UICONTROL Adobe Connect]**。

   ![](assets/event-settings-adobe-connect.png)

1. 选择您的&#x200B;**[!UICONTROL Login]** ID，然后选择您的&#x200B;**[!UICONTROL Event]**。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/event-settings-overview.png)

   太好了！ 您的Adobe Connect活动现在已与您的Marketo活动同步。

   >[!NOTE]
   >
   >Marketo发送的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >若要将人员的唯一URL插入到电子邮件中，请使用此令牌： `{{member.webinar url}}`。 在发送电子邮件时，此令牌会自动从Adobe Connect中解析人员的唯一确认URL。
   >
   >将您的确认电子邮件设置为&#x200B;**操作**，以确保注册和可能取消订阅的用户仍会收到其确认信息。

   当[!UICONTROL Change Program Status]设置为“已注册”时，注册您的网络研讨会的用户将通过[!UICONTROL New Status]流程步骤推送至您的网络研讨会提供商。 没有其他状态会将该人员推倒。 此外，请确保将[!UICONTROL Change Program Status]流程步骤#1和[!UICONTROL Send Email]流程步骤#2。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件程序发送确认电子邮件。 请改用事件项目的智能营销活动，如上所示。

   >[!TIP]
   >
   >数据可能需要48小时才能显示在Marketo中。 如果在等待了这么长时间后仍未看到任何内容，请从事件的“摘要”选项卡的“事件操作”菜单中选择&#x200B;**[!UICONTROL Refresh from Webinar Provider]**。

   >[!MORELIKETHIS]
   >
   >* [将Adobe Connect添加为 [!DNL LaunchPoint] 服务](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [编辑事件频道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
