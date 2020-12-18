---
unique-page-id: 2949865
description: 使用Adobe Connect- Marketo Docs —— 产品文档创建事件
title: 与Adobe Connect建立事件
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# 创建与Adobe Connect{#create-an-event-with-adobe-connect}的事件

与Adobe Connect同步使您能够管理Marketo内的网络研讨会注册和出席情况，确保不会失去参与。

>[!PREREQUISITES]
>
>* [链接Adobe Connect和Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [创建新事件项目](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


首先，确保已在Adobe Connect创建会议或研讨会。 如果您需要帮助，请查阅[《Adobe Connect用户指南》](http://help.adobe.com/en_US/connect/9.0/using/index.html)。 您在Adobe Connect创建的会议和研讨会必须在您在Marketo中输入凭据时指定的文件夹下创建。 在创建会议或研讨会后，记下要在确认电子邮件和ICS文件中使用的任何相关后勤信息（如电话号码）。

>[!NOTE]
>
>目前，我们&#x200B;**不**&#x200B;支持Adobe Connect现场。

1. 在新事件的主页上，选择&#x200B;**事件操作**，然后选择&#x200B;**事件设置**。

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >如果下拉框中未显示&#x200B;**事件设置**，请确保事件的渠道具有&#x200B;**事件，在“应用到”下选择了网络研讨会**。

1. 在&#x200B;**事件合作伙伴**&#x200B;下，选择&#x200B;**Adobe Connect**。

   ![](assets/event-settings-adobe-connect.png)

1. 选择&#x200B;**登录** ID，然后选择&#x200B;**事件**。

   ![](assets/event-settings-select-event-adobe-connect.png)

1. 单击&#x200B;**保存**。

   ![](assets/event-settings-overview.png)

   不错！ 您的Adobe Connect事件现在与您的Marketo事件同步。

   >[!NOTE]
   >
   >Marketo发送到的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >要在电子邮件中插入人员的唯一URL，请使用以下令牌：`{{member.webinar url}}`。 发送电子邮件时，此令牌会自动解析该人员来自Adobe Connect的唯一确认URL。
   >
   >将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册并可能取消订阅的用户仍会收到其确认信息。

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件项目发送确认电子邮件。 请改用事件项目的智能活动，如上所示。

   >[!TIP]
   >
   >数据在Marketo中显示可能需要48小时。 如果等待那么长时间后仍看不到任何内容，请从事件的“摘要”选项卡的“事件操作”菜单中选择“从网络研讨会提供者刷新”**。**

   >[!MORELIKETHIS]
   >
   > * [将Adobe Connect添加为LaunchPoint服务](../../../../product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [编辑事件渠道](../../../../product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


注册您的网络研讨会的人员将在“新状态”设置为“已注册”时，通过“更改项目状态”流程步骤推送到您的网络研讨会提供者。 没有其他状态会把人推倒。 另外，请确保更改项目状态流步骤#1和发送电子邮件流步骤#2。
