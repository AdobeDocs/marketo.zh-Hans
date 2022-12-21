---
unique-page-id: 2949865
description: 使用Adobe Connect创建事件 — Marketo文档 — 产品文档
title: 使用Adobe Connect创建事件
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 使用Adobe Connect创建事件 {#create-an-event-with-adobe-connect}

与Adobe Connect同步后，您可以在Marketo中管理网络研讨会注册和出席情况，以确保不会取消跟踪参与情况。

>[!PREREQUISITES]
>
>* [链接Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [创建新事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


首先，确保已在Adobe Connect创建会议或研讨会。 如果您需要帮助，请查看 [Adobe Connect用户指南](https://help.adobe.com/en_US/connect/9.0/using/index.html).

您在Adobe Connect中创建的会议和研讨会必须在您在Marketo中输入凭据时指定的文件夹下创建。 创建会议或研讨会后，记下要在确认电子邮件和ICS文件中使用的任何相关后勤信息（如电话号码）。

>[!CAUTION]
>
>作为事件主机，请确保从应用程序内和 **not** 通过发送给与会者的链接。

>[!NOTE]
>
>我们当前不支持Adobe Connect现场。

1. 在新活动的主页上，选择 **事件操作**，然后 **事件设置**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果你看不到 **事件设置** 在下拉列表中，确保事件的渠道 **网络研讨会活动** “Applies to”（应用于）下选择。

1. 在 **活动合作伙伴**，选择 **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. 选择 **登录** ID和 **事件**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 单击 **保存**.

   ![](assets/event-settings-overview.png)

   不错！ 您的Adobe Connect事件现在与Marketo事件同步。

   >[!NOTE]
   >
   >Marketo发送的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >要将人员的唯一URL插入电子邮件，请使用以下令牌： `{{member.webinar url}}`. 发送电子邮件后，此令牌会自动从Adobe Connect解析人员的唯一确认URL。
   >
   >将确认电子邮件设置为 **运行** 确保登记和可能被注销的人员仍收到确认信息。

   注册网络研讨会的人员在将“新状态”设置为“已注册”时，将通过更改项目状态流程步骤推送到网络研讨会提供商。 没有其他状态会将人推过去。 另外，请务必执行更改项目状态流程步骤#1和发送电子邮件流程步骤#2。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件程序发出确认电子邮件。 请改用事件项目的智能营销活动，如上所示。

   >[!TIP]
   >
   >数据可能最多需要48小时才能在Marketo中显示。 如果等待了那么长时间后仍未看到任何内容，请选择 **从网络研讨会提供商刷新** 从事件“摘要”选项卡的事件操作菜单。

   >[!MORELIKETHIS]
   >
   >* [将Adobe Connect添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [编辑事件渠道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

