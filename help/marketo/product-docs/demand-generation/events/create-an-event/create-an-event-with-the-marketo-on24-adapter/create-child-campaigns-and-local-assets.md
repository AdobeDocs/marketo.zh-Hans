---
unique-page-id: 10096675
description: 创建子活动和本地资产- Marketo文档——产品文档
title: 创建子活动和本地资产
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---


# 创建子活动和本地资产{#create-child-campaigns-and-local-assets}

使用Design Studio创建您的子活动和本地资源。

## 登陆页和表单{#landing-page-and-form}

为确保人们在ON24中正确注册，您的Marketo表单中必须包含以下字段：

* 名字
* 姓氏
* 电子邮件地址

您还可以将以下字段推送到ON24:

* 公司名称
* 职务

在注册活动中添加适当的流程步骤后，用户将被推送到ON24并标记为已注册。 您可以向表单中添加其他字段，该信息将在Marketo中作为人员详细信息记录的一部分被捕获。

>[!CAUTION]
>
>要成功进行集成，您必须使用Marketo表单来注册您的事件人员，或使用非Marketo表单来通过正确的API集成将注册数据推送到Marketo。

## 电子邮件和URL令牌{#emails-and-url-tokens}

使用Marketo创建邀请、确认、跟进和感谢电子邮件。

## Marketo确认电子邮件和URL令牌{#marketo-confirmation-email-and-url-token}

使用Market向事件发送确认电子邮件。 当人员注册时，他／她会收到用于进入事件的唯一URL。

>[!NOTE]
>
>要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌：`{{member.webinar url}}`。 当您发出确认URL时，此令牌会自动解析为个人的唯一确认URL。
>
>将确认电子邮件的类型设置为&#x200B;**Operational**，以确保注册人员接收其确认信息，即使他们已取消订阅。

>[!TIP]
>
>您可以配置ON24以发出确认、提醒或跟进电子邮件。 有关详细信息，请参见[ON24帮助站点](https://webcastelitehelp.on24.com)。

## 注册子活动要求{#registration-child-campaign-requirements}

事件包含一个或多个子活动，这些子事件可以协同工作，让人员在项目状态中移动，并让您跟踪的性能。

子活动的例子有邀请活动、注册活动和后续活动。

>[!CAUTION]
>
>要使适配器完成其工作，您必须创建注册活动。 此活动必须由填写表单的人员触发，并且第一步必须将人员的项目状态更改为&#x200B;**Registered**。 活动随后会发送确认电子邮件。 有关详细信息，请参阅本文的其余部分。

**注册／确认(触发活动)**

* 智能列表
* 触发基于&#x200B;**填写表单**。 请务必使用&#x200B;**添加约束**&#x200B;包含表单所在的登陆页，尤其是当同一表单用于多个登陆页时。

>[!CAUTION]
>
>您必须使用Marketo表单来注册您的事件人员，或使用正确的API集成的非Marketo表单来将注册数据推送到Marketo。 这对于您的事件合作伙伴集成的成功至关重要。

>[!NOTE]
>
>如果您在非Marketo登陆页上使用Marketo表单，则触发器将是&#x200B;**用表单名称填写表单**。

![](assets/image2015-12-22-15-3a20-3a51.png)

**流量**

* **更改项目状态** -设置为网络研讨会->已注册。

设置子活动时，此流步骤是FIRST FLOW STEP的必需步骤。 当人员的项目状态变为“已注册”时，Marketo会将注册信息推送到ON24。 没有其他状态会把人推倒。

* **发送电子邮件** -确认电子邮件。将此电子邮件设置为&#x200B;**Operational**，以便已注册的未订阅人员仍会收到此电子邮件。

**发送电子邮件**&#x200B;流步骤必须是第二步。 确认电子邮件包含`{{member.webinar url}}`，其中填充了从ON24发回Marketo的信息。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>这些流步骤的顺序很重要，因为操作在Marketo中的执行顺序。 **更改项目状态**&#x200B;步骤将人发送到ON24进行注册，并生成唯一URL。 发生此情况后，您可以使用`{{member.webinar URL}}`令牌发出包含此唯一URL的确认电子邮件。
>
>如果返回人员时出现注册错误，则他们将不会收到电子邮件确认。

下一步是[测试ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)。

>[!MORELIKETHIS]
>
>* [了解ON24适配器的营销事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [示例ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [了解网络研讨会项目状态](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

