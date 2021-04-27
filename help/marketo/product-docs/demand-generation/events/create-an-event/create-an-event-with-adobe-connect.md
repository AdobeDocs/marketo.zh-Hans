---
unique-page-id: 2949865
description: 使用Adobe Connect - Marketo Docs — 产品文档创建事件
title: 使用Adobe Connect创建事件
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 使用Adobe Connect {#create-an-event-with-adobe-connect}创建事件

与Adobe Connect同步可让您管理Marketo内的网络研讨会注册和出席情况，从而确保不会取消参与。

>[!PREREQUISITES]
>
>* [链接Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [创建新事件项目](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


首先，请确保您已在Adobe Connect中创建了会议或研讨会。 如果需要帮助，请查阅[《Adobe Connect用户指南》](https://help.adobe.com/en_US/connect/9.0/using/index.html)。

您在Adobe Connect中创建的会议和研讨会必须在您在Marketo中输入凭据时指定的文件夹下创建。 创建会议或研讨会后，请记下要在确认电子邮件和ICS文件中使用的任何相关后勤信息（如电话号码）。

>[!CAUTION]
>
>作为事件主持人，请确保通过发送给与会者的链接从应用程序内加入，而&#x200B;**不**。

>[!NOTE]
>
>我们目前不支持Adobe Connect现场服务。

1. 在新事件的主页上，选择&#x200B;**事件操作**，然后选择&#x200B;**事件设置**。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果您在下拉列表中未看到&#x200B;**事件设置**，请确保事件的渠道在“应用到”下选择了&#x200B;**网络研讨会**&#x200B;事件。

1. 在&#x200B;**事件合作伙伴**&#x200B;下，选择&#x200B;**Adobe Connect**。

   ![](assets/event-settings-adobe-connect.png)

1. 选择&#x200B;**登录** ID，然后选择&#x200B;**事件**。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 单击&#x200B;**保存**。

   ![](assets/event-settings-overview.png)

   不错！ 您的Adobe Connect事件现已与Marketo事件同步。

   >[!NOTE]
   >
   >Marketo发送的字段有：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >要在电子邮件中插入个人的唯一URL，请使用以下令牌：`{{member.webinar url}}`。 发送电子邮件时，此令牌会自动解析该人员的唯一确认URL，该URL来自Adobe Connect。
   >
   >将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册并可能取消订阅的人员仍会收到其确认信息。

   注册您的网络研讨会的人员将在“新状态”设置为“已注册”时，通过“更改项目状态”流程步骤推送到您的网络研讨会提供商。 没有其他状态会推倒此人。 另外，请务必使“更改项目状态”流程步骤#1和“发送电子邮件流程”#2。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用嵌套的电子邮件项目发送您的确认电子邮件。 请改用事件项目的智能活动，如上所示。

   >[!TIP]
   >
   >数据在Marketo中显示可能需要48小时。 如果等待了那么久，您仍然看不到任何内容，请从您的事件的“摘要”选项卡的“事件操作”菜单中选择“从网络研讨会提供者刷新”。****

   >[!MORELIKETHIS]
   >
   >* [将Adobe Connect添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [编辑事件渠道](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)

