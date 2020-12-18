---
unique-page-id: 2949863
description: 使用WebEx - Marketo Docs —— 产品文档创建事件
title: 使用WebEx创建事件
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 0%

---


# 使用WebEx {#create-an-event-with-webex}创建事件

>[!PREREQUISITES]
>
>* [将WebEx添加为LaunchPoint服务](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [创建新事件项目](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* 设置适当的[流动操作](http://docs.marketo.com/display/DOCS/Flow+Actions)以跟踪参与情况


首先在WebEx事件中心创建Webex事件。 Marketo仅使用特定设置和字段进行集成，我们很快将会通过这些设置和字段。 您可能要为WebEx配置的其他字段在[WebEx事件中心用户指南](http://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf)中进行说明。

## 基本信息{#basic-information}

* **事件名** 称——此名称将在Marketo中查看。
* **未列出的复选框**

   * 建议您&#x200B;**不要**&#x200B;列表事件。 这将确保所有人员通过您的营销登陆页注册。 通过Marketo以外的机制注册的人员在事件结束后将在Marketo中显示，并且仅当他们参加了事件。
   * 如果您选择列表事件，该列表将显示在访问您的事件中心网站的任何人的事件页面上。

* **注册-** 选中此框可设置为“必需”。您将使用Marketo表单/登陆页来捕获将推送到WebEx的注册信息。
* **事件口令**-（可选）如果您使用此字段，请确保在确认电子邮件中包含它！

![](assets/image2015-5-28-13-3a30-3a55.png)

## 日期和时间{#date-time}

* **开始日** -输入开始日期。这将在Marketo中查看。

* **开始时间** -输入您的开始时间。这将在Marketo中查看。

* **估计持续时间** -指定事件的持续时间。这将在Marketo中查看。

* **时区** -输入适用的时区。他们将在Marketo中查看。

![](assets/image2015-5-28-13-3a37-3a39.png)

## 音频会议设置{#audio-conference-settings}

这些设置仅驻留在WebEx中。 它们不被Marketo使用或查看，但可能对您的网络研讨会很重要，请多次检查它们！

## 事件描述和选项{#event-description-options}

以下选项供Marketo使用或查看。 其他字段仅驻留在WebEx中。

* **说明** -输入说明。这在Marketo中是可查看的，但不可修改。
* **事件后调查** - Marketo目前无法在WebEx事件后调查上捕获信息。
* **目标URL** -（可选）您可以输入Marketo登陆页的URL，作为会话结束后显示的目标URL。

![](assets/image2015-5-28-13-3a48-3a49.png)

## 与会者和注册{#attendees-registration}

您将使用Marketo列表控制邀请事件、注册表单和其他电子邮件。 Marketo不支持其他功能，包括：

* **最大注册者数** -当 **** 前不支持使用Marketo-WebEx集成。在Marketo中，可以使用“待批准”进度状态手动审批注册者。

* **需要注册ID**  —— 当前支持使用Marketo-WebEx集成。您可以使用Market向事件发送确认电子邮件。 当人员注册时，他们会收到用于输入事件的唯一URL。

   >[!TIP]
   >
   >要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 发出确认URL时，此令牌会自动解析为个人的唯一确认URL。
   >
   >将您的确认电子邮件设置为&#x200B;**Operational**，以确保注册并可能取消订阅的用户仍会收到其确认信息。

* **注册密码** -（可选）当前不支持使用Marketo-WebEx集成。
* **批准规则** -当前不支持使用Marketo-WebEx集成。但是，您可以在Market中使用智能活动来控制审批。

![](assets/image2015-5-28-14-3a4-3a41.png)

### 演示者和专题讨论成员{#presenters-panelists}

本节中配置的信息不会传递给Marketo。

### 电子邮件{#email-messages}

您将使用Market向注册者发送电子邮件、确认电子邮件等。 您无需在此部分中配置任何内容。 在WebEx中禁用（取消选中）电子邮件选项。

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Marketo-WebEx集成不支持从WebEx发送确认电子邮件。 确认必须通过Marketo发送。 安排事件后，请务必将事件信息复制到Marketo确认电子邮件中，并将该电子邮件设置为&#x200B;**Operational**。

现在，我们准备进入Marketo!

1. 选择您创建的事件。 打开&#x200B;**事件操作**&#x200B;下拉框。 选择&#x200B;**事件设置。**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >所选渠道的事件类型必须为&#x200B;**网络研讨会**。

1. 在&#x200B;**事件合作伙伴**&#x200B;下，选择&#x200B;**WebEx**。

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. 在&#x200B;**登录**&#x200B;下，选择WebEx登录名。

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. 在&#x200B;**事件**&#x200B;下，选择新创建的WebEx事件。 然后，选择可选的备份页面，然后单击&#x200B;**保存**。

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. 为WebEx事件选择可选的备份页面。 从已批准的营销人员登陆页的下拉列表中选择，或输入非营销人员登陆页的URL。

   >[!TIP]
   >
   >如果成员在事件事件时间之前单击其自定义开始URL，请设置备份页面以将其定向到特定页面。

   >[!NOTE]
   >
   >Marketo发送到的字段包括：名字、姓氏、电子邮件地址。

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >避免使用嵌套电子邮件项目发送确认电子邮件。 请改用事件项目的智能活动，如上所示。

   >[!TIP]
   >
   >数据在Marketo中显示可能需要48小时。 如果等待那么长时间后仍看不到任何内容，请从事件的&#x200B;**摘要**&#x200B;选项卡的“事件操作”菜单中选择&#x200B;**从网络研讨会提供者**&#x200B;刷新。

真贴心！ 您的WebEx事件现在与您的Marketo事件同步。  注册您的网络研讨会的人员将在“新状态”设置为“已注册”时，通过“更改项目状态”流程步骤推送到您的网络研讨会提供者。 没有其他状态会把人推倒。 另外，请确保更改项目状态流步骤#1和发送电子邮件流步骤#2。

## 查看计划{#viewing-the-schedule}

在[项目计划视图](http://docs.marketo.com/display/docs/program+schedule+view)中，单击事件的日历条目。 您可以在屏幕右侧看到计划!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>要更改事件计划，您需要在WebEx上编辑网络研讨会。
