---
unique-page-id: 2949865
description: 使用Adobe Connect创建事件 — Marketo文档 — 产品文档
title: 使用Adobe Connect创建事件
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 使用Adobe Connect创建事件 {#create-an-event-with-adobe-connect}

与Adobe Connect同步允许您在Marketo中管理网络研讨会的注册和出席情况，从而确保参与情况不会被取消跟踪。

>[!PREREQUISITES]
>
>* [链接Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [创建新的事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

首先，确保您已在Adobe Connect中创建了会议或研讨会。 如果您需要帮助，请查看 [Adobe Connect用户指南](https://help.adobe.com/en_US/connect/9.0/using/index.html).

您在Adobe Connect中创建的会议和研讨会必须在您在Marketo中输入凭据时指定的文件夹下创建。 创建会议或研讨会后，记下任何相关的后勤信息（如电话号码），以便在确认电子邮件和ICS文件中使用。

>[!CAUTION]
>
>作为事件主机，请确保从应用程序中加入，并且 **非** 通过发送给与会者的链接。

>[!NOTE]
>
>我们目前不支持现场Adobe Connect。

1. 在新事件的主页上，选择 **事件操作**，然后 **事件设置**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果您没有看到 **事件设置** 在下拉菜单中，确保事件的渠道具有 **网络研讨会活动** 在“应用于”下选中。

1. 下 **活动合作伙伴**，选择 **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. 选择您的 **登录** ID并选择 **事件**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 单击 **保存**.

   ![](assets/event-settings-overview.png)

   很好！ 您的Adobe Connect事件现在已与您的Marketo事件同步。

   >[!NOTE]
   >
   >Marketo发送的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >要将人员的唯一URL插入到电子邮件中，请使用此令牌： `{{member.webinar url}}`. 在发送电子邮件时，此令牌会自动从Adobe Connect中解析人员的唯一确认URL。
   >
   >将确认电子邮件设置为 **可操作** 以确保已注册和可能取消订阅的用户仍会收到其确认信息。

   当新状态设置为“已注册”时，注册您的网络研讨会的用户将通过“更改计划状态”流程步骤推送到您的网络研讨会提供商。 没有其他状态会将人员推到。 此外，请确保将“更改项目状态”流程步骤#1和“发送电子邮件流程”步骤#2设置为。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件程序发送确认电子邮件。 请改用事件程序的智能营销活动，如上所示。

   >[!TIP]
   >
   >数据可能需要48小时才能显示在Marketo中。 如果在等待了那么长时间后仍未看到任何内容，请选择 **从网络研讨会提供商刷新** 从事件的“摘要”选项卡中的“事件操作”菜单。

   >[!MORELIKETHIS]
   >
   >* [将Adobe Connect添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [编辑事件渠道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
