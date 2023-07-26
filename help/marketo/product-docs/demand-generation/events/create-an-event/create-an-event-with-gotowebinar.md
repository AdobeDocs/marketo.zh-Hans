---
unique-page-id: 2949874
description: 通过转至网络研讨会创建事件 — Marketo文档 — 产品文档
title: 使用GotoWebinar创建事件
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 使用GotoWebinar创建事件 {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [将GoToWebinar添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [创建新的事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的 [流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)以跟踪参与情况

首先在GoToWebinar中创建网络研讨会。 GoTo网络研讨会创建过程中的某些设置由Marketo使用，而某些设置仅由GoTo网络研讨会使用。

在您创建Marketo活动并将GoToWebinar与其关联后，系统将能够共享注册和出席信息。

以下是Marketo使用的设置列表。

## 标题和描述 {#title-and-description}

**网络研讨会名称**  — 输入网络研讨会的名称。 此名称将显示在Marketo中。

**描述** （可选） — 输入网络研讨会的说明。 该描述将显示在Marketo中。

![](assets/image2015-5-28-15-3a1-3a36.png)

## 日期和时间 {#date-time}

为您的网络研讨会输入以下信息，这些信息将通过适配器拉入Marketo。 如果您对此信息进行了任何更改，则必须单击链接&#39;&#39;**从网络研讨会提供商刷新**“，在 **事件操作**，以便Marketo查看更改情况。

**开始日期**  — 输入开始日期。 该屏幕将显示在Marketo中。

**开始时间**  — 输入您的开始时间。 该屏幕将显示在Marketo中。

**结束时间**  — 输入您的结束时间。 该屏幕将显示在Marketo中。

**时区**  — 选择适用的时区。 该可视化图表将在Marketo中可见。

**类型 —** 设置为 **一个会话**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo当前不支持定期网络研讨会。 在每个Marketo活动与GoToWebinar网络研讨会之间，必须设置一个会话。

>[!TIP]
>
>如果您需要其他GoTo网络研讨会帮助，请访问 [帮助站点](https://support.logmeininc.com/gotowebinar).

现在，让我们跳入Marketo！

1. 选择一个事件。 单击 **事件操作** 并选择 **事件设置**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >所选事件的渠道类型必须为 **网络研讨会**.

1. 选择 **GoTo网络研讨会** 从 **活动合作伙伴** 列表。

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. 选择帐户。

   ![](assets/rtaimage-2.png)

1. 选择网络研讨会。

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. 单击 **保存**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. 太棒了！ 现在，该事件已由同步并计划 **GoTo网络研讨会**.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Marketo发送的字段包括：名字、姓氏、电子邮件地址。 这些字段为必填项，不得为空。

   >[!TIP]
   >
   >要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌： `{{member.webinar url}}`. 在发送确认URL时，此令牌会自动解析为人员的唯一确认URL。
   >
   >将确认电子邮件设置为 **可操作** 以确保已注册和可能取消订阅的人员仍会收到其确认信息。

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件程序发送确认电子邮件。 请改用事件项目的智能营销活动，如上所示。

   >[!TIP]
   >
   >数据可能需要48小时才能显示在Marketo中。 如果经过这么长的时间后仍未看到任何内容，请选择 **从网络研讨会提供商刷新** 从“事件操作”菜单 **摘要** 选项卡。

当新状态设置为“已注册”时，注册您的网络研讨会的用户将通过“更改项目状态”流程步骤推送至您的网络研讨会提供商。 没有其他状态会将该人员推倒。 此外，请确保将“更改项目状态”流程步骤#1和“发送电子邮件”流程步骤#2设置为。

## 查看计划  {#viewing-the-schedule}

在项目计划视图中，单击事件的日历条目。 您可以在屏幕右侧查看计划。

>[!NOTE]
>
>若要更改您的活动计划，您需要在GoTo网络研讨会上编辑网络研讨会。

![](assets/image2015-5-14-15-3a3-3a13.png)
