---
unique-page-id: 2949863
description: 使用Webex创建事件 — Marketo文档 — 产品文档
title: 使用Webex创建事件
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 使用Webex创建事件 {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [将Webex添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [创建新的事件程序](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的 [流程操作](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) 以跟踪参与情况
>* 确保您使用的是Webex Events (classic)

首先在Webex活动中心创建Webex活动。 Marketo仅为您的集成使用特定的设置和字段，我们很快将介绍这些设置和字段。 有关您可能需要为Webex配置的其他字段的说明，请参见 [Webex活动中心用户指南](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketo Engage仅支持在Webex Events (classic)中创建的事件。 目前，Marketo不支持在Webex事件（新）中创建的事件。

## 基本信息 {#basic-information}

* **事件名称 —** 此名称将显示在Marketo中。
* **未列出的复选框**

   * 建议您最好这样做 **非** 列出您的活动。 这将确保所有人都通过您的Marketo登陆页面进行注册。 通过Marketo以外的机制注册的人员，将在活动结束后且仅当他们参加活动时，才会显示在Marketo中。
   * 如果选择列出事件，该事件将显示在访问您事件中心网站的任何人的“事件列表”页面中。

* **注册 —** 选中此框可将其设置为“必需”。 您将使用Marketo表单/登陆页面来捕获将推送到Webex的注册信息。
* **事件密码** — （可选）如果您使用此字段，请确保将其包含在确认电子邮件中！

![](assets/image2015-5-28-13-3a30-3a55.png)

## 日期和时间 {#date-time}

* **开始日期**  — 输入开始日期。 该屏幕将显示在Marketo中。

* **开始时间**  — 输入您的开始时间。 该屏幕将显示在Marketo中。

* **估计持续时间**  — 指定事件的持续时间。 该屏幕将显示在Marketo中。

* **时区**  — 输入适用的时区。 它们可以在Marketo中查看。

![](assets/image2015-5-28-13-3a37-3a39.png)

## 音频会议设置 {#audio-conference-settings}

这些设置仅位于Webex中。 它们不能在Marketo中使用或查看，但它们可能对您的网络研讨会很重要，因此请仔细检查它们！

## 事件描述和选项  {#event-description-options}

以下选项由使用或者可以在Marketo中查看。 其他字段仅位于Webex中。

* **描述**  — 输入说明。 此操作可以在Marketo中查看但不能修改。
* **事件后调查** -Marketo目前无法捕获Webex事件后调查中的信息。
* **目标URL**  — （可选）您可以输入Marketo登陆页面的URL，以用作会话结束后显示的目标URL。

![](assets/image2015-5-28-13-3a48-3a49.png)

## 出席者和注册 {#attendees-registration}

您将通过Marketo活动来控制邀请列表、注册表单和其他电子邮件。 Marketo不支持其他功能，包括：

* **最大注册者数**  — 当前 **非** 通过Marketo-Webex集成支持。  可以使用Marketo中的未决批准进度状态来手动批准注册者。

* **需要注册ID**  — 当前支持使用Marketo-Webex集成。 您可以使用Marketo发送事件的确认电子邮件。 人员注册时，会收到用于输入事件的唯一URL。

  >[!TIP]
  >
  >要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌： `{{member.webinar url}}`. 在发送确认URL时，此令牌会自动解析为人员的唯一确认URL。
  >
  >将确认电子邮件设置为 **可操作** 以确保已注册和可能取消订阅的人员仍会收到其确认信息。

* **注册密码**  — （可选）当前不支持使用Marketo-Webex集成。
* **批准规则**  — 当前不支持使用Marketo-Webex集成。 但是，您可以在Marketo中使用智能营销活动来控制审批。

![](assets/image2015-5-28-14-3a4-3a41.png)

### 演示者和小组成员 {#presenters-panelists}

此部分中配置的信息未传递到Marketo。

### 电子邮件 {#email-messages}

您将使用Marketo向注册者发送电子邮件、确认电子邮件等。 您无需在此部分中配置任何内容。 禁用（取消选中）Webex中的电子邮件选项。

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Marketo-Webex集成不支持从Webex发送确认电子邮件。 确认必须通过Marketo发送。 计划活动后，请确保将活动信息复制到Marketo确认电子邮件中，并将电子邮件设置为 **可操作**.

现在我们准备跳入Marketo了！

1. 选择您创建的事件。 打开 **事件操作** 下拉菜单。 选择 **事件设置。**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >所选事件的渠道类型必须为 **网络研讨会**.

1. 下 **活动合作伙伴**，选择 **Webex**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. 下 **登录**，选择您的Webex登录名。

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. 下 **事件**，选择您新创建的Webex事件。 然后，选择可选的“备份”页并单击 **保存**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. 为Webex事件选择可选的“备份页”。 从已批准的Marketo登陆页面的下拉菜单中选择或输入非Marketo登陆页面的URL。

   >[!TIP]
   >
   >设置一个备份页面，当成员在事件的开始时间之前单击其自定义事件URL时，将成员定向到特定页面。

   >[!NOTE]
   >
   >Marketo发送的字段包括：名字、姓氏、电子邮件地址。

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件程序发送确认电子邮件。 请改用事件项目的智能营销活动，如上所示。

   >[!TIP]
   >
   >数据可能需要48小时才能显示在Marketo中。 如果经过这么长的时间后仍未看到任何内容，请选择 **从网络研讨会提供商刷新** 从“事件操作”菜单 **摘要** 选项卡。

真贴心！ 您的Webex活动现在已与您的Marketo活动同步。 当新状态设置为“已注册”时，注册您的网络研讨会的用户将通过“更改项目状态”流程步骤推送至您的网络研讨会提供商。 没有其他状态会将该人员推倒。 此外，请确保将“更改项目状态”流程步骤#1和“发送电子邮件”流程步骤#2设置为。

## 查看计划  {#viewing-the-schedule}

在项目计划视图中，单击事件的日历条目。 您可以在屏幕右侧查看计划！

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>要更改您的活动计划，您需要在Webex上编辑网络研讨会。
