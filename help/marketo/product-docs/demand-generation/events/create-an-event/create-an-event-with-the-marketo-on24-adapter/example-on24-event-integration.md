---
unique-page-id: 10096679
description: 24事件集成示例 — Marketo文档 — 产品文档
title: ON24事件集成示例
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# ON24事件集成示例 {#example-on-event-integration}

以下是ON24网络研讨会的示例活动，包括营销活动。 构建事件时，请务必先测试营销活动，然后再运行营销活动。

## 在营销活动中创建新事件 {#create-a-new-event-in-marketing-activities}

1. 选择 **新建** > **新计划**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. 选择 **Campaign文件夹** 活动的位置。

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. 输入 **名称** 的值。

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. 选择 **事件** 作为 **程序类型**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. 选择 **网络研讨会** 作为 **渠道** 的值。

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. 单击&#x200B;**创建**。

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## 邀请（批量营销活动）  {#invite-batch-campaign}

* **智能列表**  — 定义邀请谁参加该活动。
* **流量**

   * 发送电子邮件 — 如果这是本地资产电子邮件，则其将遵循以下命名约定：EventName.EmailName。 您还可以使用全局电子邮件。
   * 按进度更改状态 — 设置为网络研讨会>受邀。

* **计划**  — 设置发送邀请的日期。

## 注册/确认（触发营销活动） {#registration-confirmation-trigger-campaign}

* **智能列表**

   * 根据 **填写表单**. 请务必使用 **添加约束**，尤其是当表单用于多个登陆页面时。

>[!CAUTION]
>
>您必须使用Marketo表单为事件注册人员，或使用正确API集成的非Marketo表单将注册数据推送到Marketo。 这对于活动合作伙伴集成的成功至关重要。 **注意**:如果您在非Marketo登陆页面上使用Marketo表单，则触发器将为 **填写表单** ，其中包含“表单名称”。

![](assets/image2015-12-22-15-3a50-3a22.png)

* **流量**

   * **按进度更改状态**  — 设置为网络研讨会>已注册。 **注意**:设置子营销活动时，需要执行此流程步骤。 当人员的晋升状态更改为 **已注册**,Marketo将注册信息推送到ON24。

   * **发送电子邮件**  — 确认电子邮件(设置为 **运行** 这样，注册的未注册用户仍然会收到它)。

![](assets/image2015-12-22-15-3a52-3a9.png)

**注意**:如果返回人员时出现注册错误，则他们将不会收到电子邮件确认。

## 提醒（批量营销活动） {#reminder-batch-campaign}

* **智能列表**  — 使用 **方案成员** 并将状态设置为 **已注册**.

* **流量**  — 发送电子邮件（提醒电子邮件）。

**注意**:您可以使用类似的营销活动发送 *不同* 向受邀但尚未注册的人员发送跟进电子邮件。

## 后续促销活动（批量或触发促销活动） {#follow-up-campaign-batch-or-trigger-campaign}

* **智能列表**  — 根据程序状态的更改触发。

![](assets/image2015-12-22-15-3a57-3a25.png)

* **流量**  — 发送电子邮件。 根据项目状态，使用选项发送不同的电子邮件。

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}
