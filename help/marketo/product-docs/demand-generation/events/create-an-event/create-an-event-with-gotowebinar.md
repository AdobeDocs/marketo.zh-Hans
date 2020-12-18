---
unique-page-id: 2949874
description: 使用GotoWebinar - Marketo Docs —— 产品文档创建事件
title: 使用GotoWebinar创建事件
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# 使用GotoWebinar {#create-an-event-with-gotowebinar}创建事件

>[!PREREQUISITES]
>
>* [将GoToWebinar添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [创建新事件项目](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的[流动操作](http://docs.marketo.com/display/DOCS/Flow+Actions)以跟踪参与情况


首先在GoToWebinar中创建网络研讨会。 在您创建GoToWebinar时，某些设置由Marketo使用，有些设置仅由GoToWebinar使用。

在您创建营销人员事件并将GoTo网络研讨会与其关联后，系统将能够共享注册和出席信息。 有关创建GoToWebinar的帮助，请参阅[GoToWebinar用户指南](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf)。

以下是Marketo使用的设置列表。

## 标题和说明{#title-and-description}

**网络研讨会名** 称——输入网络研讨会的名称。此名称将在Marketo中查看。

**说明** （可选）-输入网络研讨会的说明。描述将可在Marketo中查看。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日期和时间{#date-time}

`Enter the following information for your webinar and it will be pulled into Marketo via the`适配器。如果对此信息做了任何更改，则必须单击&#x200B;**事件操作**&#x200B;下的“从网络研讨会提供者刷新&#x200B;**”链接，以便Market能够看到这些更改。**

**开始日** -输入开始日期。这将在Marketo中查看。

**开始时间** -输入您的开始时间。这将在Marketo中查看。

**结束时间** -输入您的结束时间。这将在Marketo中查看。

**时区** -选择适用的时区。它将在Marketo中查看。

**键入-** 设置 **为“One Session**”。

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo当前不支持重复的网络研讨会。 您必须在每个营销人员事件和GoTo网络研讨会之间设置一个会话。

>[!TIP]
>
>您将在GoToWebinar中配置其他字段，这些字段不会影响集成。 请参阅[GoToWebinar用户指南](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf)以了解有关这些字段的更多信息，因为本文不会介绍这些字段。 如果您需要其他GoToWebinar帮助，请访问其[帮助站点](http://support.logmeininc.com/gotowebinar)。

现在，让我们跳进市场！

1. 选择事件。 单击&#x200B;**事件操作**，然后选择&#x200B;**事件设置**。

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >所选渠道的事件类型必须为&#x200B;**网络研讨会**。

1. 从&#x200B;**事件** **合作伙伴**&#x200B;列表中选择&#x200B;**GoToWebinar**。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. 选择帐户。

   ![](assets/rtaimage-2.png)

1. 选择网络研讨会。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 单击&#x200B;**保存**。

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 太棒了！ 现在，事件由&#x200B;**GoToWebinar**&#x200B;同步并计划。

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Marketo发送到的字段包括：名字、姓氏、电子邮件地址。 这些字段为必填字段，不得为空。

   >[!TIP]
   >
   >要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 发出确认URL时，此令牌会自动解析为个人的唯一确认URL。
   >
   >将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册并可能取消订阅的用户仍会收到其确认信息。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件项目发送确认电子邮件。 请改用事件项目的智能活动，如上所示。

   >[!TIP]
   >
   >数据在Marketo中显示可能需要48小时。 如果等待那么长时间后仍看不到任何内容，请从事件的&#x200B;**摘要**&#x200B;选项卡的“事件操作”菜单中选择&#x200B;**从网络研讨会提供者**&#x200B;刷新。

注册您的网络研讨会的人员将在“新状态”设置为“已注册”时，通过“更改项目状态”流程步骤推送到您的网络研讨会提供者。 没有其他状态会把人推倒。 另外，请确保更改项目状态流步骤#1和发送电子邮件流步骤#2。

## 查看计划{#viewing-the-schedule}

在[项目计划视图](http://docs.marketo.com/display/docs/program+schedule+view)中，单击事件的日历条目。 您可以在屏幕右侧看到计划。

>[!NOTE]
>
>要更改事件计划，您需要在GoToWebinar上编辑网络研讨会。

![](assets/image2015-5-14-15-3a3-3a13.png)
