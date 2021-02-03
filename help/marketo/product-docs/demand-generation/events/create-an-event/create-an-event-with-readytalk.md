---
unique-page-id: 2949870
description: 使用ReadyTalk - Marketo Docs —— 产品文档创建事件
title: 使用ReadyTalk创建事件
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# 使用ReadyTalk {#create-an-event-with-readytalk}创建事件

>[!PREREQUISITES]
>
>* [将ReadyTalk添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [创建新事件项目](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的[流动操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以跟踪参与情况


首先在ReadyTalk会议中心设置事件。 如果需要帮助，请查看[ReadyTalk资源中心](https://www.readytalk.com/resources/readytalk)。 选择注册类型时，请选择&#x200B;**在会议**&#x200B;之前预先注册。 如果您在会议&#x200B;_时选择_&#x200B;注册，Marketo将&#x200B;**不**&#x200B;为您的人员捕获“已注册”状态，并且只会在网络研讨会结束&#x200B;_后拉入“已参加”状态_。

取消选中&#x200B;**通过电子邮件**&#x200B;通知我有新注册。

![](assets/image2015-5-28-21-3a18-3a39.png)

如果您使用ReadyTalk发送确认电子邮件，则还需要添加说明。 完成后，在ReadyTalk中保存事件。

>[!NOTE]
>
>要计划操作员辅助事件，请单击会议中心主屏幕左侧的&#x200B;**请求事件服务**&#x200B;链接，与我们的事件团队计划事件。

现在，您已准备好将事件关联到Marketo。

1. 选择您的事件，然后单击&#x200B;**事件操作**，最后单击&#x200B;**事件设置。**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >所选渠道的事件类型必须为&#x200B;**网络研讨会。**

1. 在&#x200B;**事件合作伙伴下，**&#x200B;选择&#x200B;**ReadyTalk**。

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. 在&#x200B;**登录下，**&#x200B;选择您的ReadyTalk登录名。

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. 在&#x200B;**事件**&#x200B;下，选择要链接的事件，然后单击&#x200B;**保存**。

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   不错！ 您的事件现已同步。

   >[!NOTE]
   >
   >Marketo发送到的字段包括：名字、姓氏、电子邮件地址。

   >[!TIP]
   >
   >要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 发出确认URL时，此令牌会自动解析为个人的唯一确认URL。
   >
   >将您的确认电子邮件设置为“运营”，以确保注册人员（可能未订阅）收到其确认信息。

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件项目发送确认电子邮件。 请改用事件项目的智能活动，如上所示。

   >[!TIP]
   >
   >数据在Marketo中显示可能需要48小时。 如果等待那么长时间后仍看不到任何内容，请从事件的&#x200B;**摘要**&#x200B;选项卡的“事件操作”菜单中选择&#x200B;**从网络研讨会提供者**&#x200B;刷新。

## 查看计划{#viewing-the-schedule}

在项目计划视图中，单击事件的日历条目。 您可以在屏幕右侧看到计划!

![](assets/image2015-5-18-12-9-58.png)

注册您的网络研讨会的人员将在“新状态”设置为“已注册”时，通过“更改项目状态”流程步骤推送到您的网络研讨会提供者。 没有其他状态会把人推倒。 另外，请确保更改项目状态流步骤#1和发送电子邮件流步骤#2。
