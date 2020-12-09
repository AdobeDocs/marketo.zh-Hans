---
unique-page-id: 10096679
description: 示例ON24事件集成- Marketo Docs —— 产品文档
title: 示例ON24事件集成
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# 示例ON24事件集成 {#example-on-event-integration}

以下是ON24网络研讨会的示例事件，包括活动。 构建事件时，请确保在运行活动之前对其进行测试。

## 在营销活动中创建新事件 {#create-a-new-event-in-marketing-activities}

1. 选择 **新建** >新 **建项目**。

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. 选择活动 **所在的事件文** 件夹。

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. 输入 **事件** 的名称。

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. 选择**事件**作为 **项目类型**。

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. 选择**网络研讨会**作为**渠道**作为事件。

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. 单击 **创建**。

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## 邀请(批活动)  {#invite-batch-campaign}

* **智能列表** -定义您将邀请谁加入事件。
* **流量**

   * 发送电子邮件——如果这是本地资产电子邮件，则其将遵循以下命名规范：EventName.EmailName。 您还可以使用全局电子邮件。
   * 更改进度状态——设置为“网络研讨会”>“已邀请”。

* **计划** -设置要发送邀请的日期。

## 注册／确认(触发活动) {#registration-confirmation-trigger-campaign}

* **智能列表**

   * 根据填写表单 **触发活动**。 请务必通过使用添加约束来包含表单所 **在的登陆页**，尤其是当表单用于多个登陆页时。

>[!CAUTION]
>
>您必须使用Marketo表单来注册事件人员，或使用正确的API集成的非Marketo表单来将注册数据推送到Marketo。 这对于您的事件合作伙伴集成的成功至关重要。 **注意**:如果您在非Marketo登陆页上使用Marketo表单，则触发器将 **是使用表单名** “填写表单”。

![](assets/image2015-12-22-15-3a50-3a22.png)

* **流量**

   * **按进度更改状态** -设置为“网络研讨会”>“已注册”。 **警告**:设置子活动时需要此流步骤。 当人员的晋升状态变为“已注 **册**”时，Marketo会将注册信息推送到ON24。

   * **发送电子邮件** -确认电子邮件(设置为 **“操作** ”，这样已注册的取消订阅的人员仍会收到该电子邮件)。

![](assets/image2015-12-22-15-3a52-3a9.png)

**注意**:如果返回人员时出现注册错误，则他们将不会收到电子邮件确认。

## 提醒(批活动) {#reminder-batch-campaign}

* **智能列表** -使用项目 **成员进行过滤** ，并将状态设置为“已 **注册”**。

* **流程** -发送电子邮件（提醒电子邮件）。

**注意**:您可以使用类似的活动向 *受邀但* 尚未注册的人发送不同的后续电子邮件。

## 后续活动(批或触发活动) {#follow-up-campaign-batch-or-trigger-campaign}

* **智能列表** -根据项目状态的更改触发。

![](assets/image2015-12-22-15-3a57-3a25.png)

* **流程** -发送电子邮件。 根据项目状态使用选项发送不同的电子邮件。

![](assets/ten.png)

>[!MORELIKETHIS]
>
>* [了解ON24适配器的营销事件](understanding-marketo-on24-adapter-events.md)

>



