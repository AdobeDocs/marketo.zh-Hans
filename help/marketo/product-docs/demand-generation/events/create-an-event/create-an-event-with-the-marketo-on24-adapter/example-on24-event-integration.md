---
unique-page-id: 10096679
description: ON24事件集成示例 — Marketo文档 — 产品文档
title: ON24事件集成示例
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# ON24事件集成示例 {#example-on-event-integration}

以下是ON24网络研讨会的示例事件（包括促销活动）。 在构建活动时，请确保在运行活动之前对其进行测试。

## 在营销活动中创建新事件 {#create-a-new-event-in-marketing-activities}

1. 选择&#x200B;**新建** > **新建程序**。

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. 选择活动将所在的&#x200B;**Campaign文件夹**。

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. 输入事件的&#x200B;**名称**。

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. 选择&#x200B;**Event**&#x200B;作为&#x200B;**程序类型**。

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. 选择&#x200B;**网络研讨会**&#x200B;作为事件的&#x200B;**渠道**。

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## 邀请（批量营销活动）  {#invite-batch-campaign}

* **智能列表** — 定义您将邀请谁参加活动。
* **流量**

   * 发送电子邮件 — 如果这是本地资产电子邮件，则它将具有以下命名约定：EventName.EmailName。 您还可以使用全局电子邮件。
   * 进度中的更改状态 — 设置为“网络研讨会”>“已邀请”。

* **计划** — 设置发送邀请的日期。

## 注册/确认（触发营销活动） {#registration-confirmation-trigger-campaign}

* **智能列表**

   * 根据&#x200B;**填写表单**&#x200B;触发营销活动。 确保使用&#x200B;**添加约束**&#x200B;来包含表单所在的登陆页面，尤其是表单用于多个登陆页面时。

>[!CAUTION]
>
>您必须使用Marketo表单注册事件用户，或使用具有正确API集成的非Marketo表单将注册数据推送到Marketo。 这对于成功集成Event Partner至关重要。 **注意**：如果您在非Marketo登录页面上使用Marketo表单，则触发器将为&#x200B;**使用表单名称**&#x200B;填写表单。

![](assets/image2015-12-22-15-3a50-3a22.png)

* **流量**

   * **在Progression**&#x200B;中更改状态 — 设置为“网络研讨会”>“已注册”。 **注意**：在设置子营销活动时，需要此流程步骤。 当人员的进度状态更改为&#x200B;**已注册**&#x200B;时，Marketo会将注册信息推送到ON24。

   * **发送电子邮件** — 确认电子邮件（设置为&#x200B;**操作**，以便已注册的已取消订阅的用户仍可接收该电子邮件）。

![](assets/image2015-12-22-15-3a52-3a9.png)

**注意**：如果返回人员时存在注册错误，则不会收到电子邮件确认。

## 提醒（批量营销活动） {#reminder-batch-campaign}

* **智能列表** — 使用&#x200B;**程序成员**&#x200B;进行筛选，并将状态设置为&#x200B;**已注册**。

* **流量** — 发送电子邮件（提醒电子邮件）。

**注意**：您可以使用类似的促销活动向受邀但尚未注册的用户发送一个&#x200B;*不同的*&#x200B;跟进电子邮件。

## 跟进营销活动（批量或触发营销活动） {#follow-up-campaign-batch-or-trigger-campaign}

* **智能列表** — 根据程序状态的更改进行触发。

![](assets/image2015-12-22-15-3a57-3a25.png)

* **流量** — 发送电子邮件。 根据项目状态使用选项发送不同的电子邮件。

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
