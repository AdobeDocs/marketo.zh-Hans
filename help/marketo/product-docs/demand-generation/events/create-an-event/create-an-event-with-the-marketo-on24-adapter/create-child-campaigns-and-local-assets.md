---
unique-page-id: 10096675
description: 创建子营销活动和本地资源 — Marketo文档 — 产品文档
title: 创建子营销活动和本地资源
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# 创建子营销活动和本地资源 {#create-child-campaigns-and-local-assets}

使用Design Studio创建子营销活动和本地资源。

## 登陆页面和表单 {#landing-page-and-form}

为确保用户正确注册ON24，您的Marketo表单中必须包含以下字段：

* 名
* 姓
* 电子邮件地址

您还可以将以下字段推送到ON24：

* 公司名称
* 职务

向注册活动添加适当的流程步骤后，用户将被推送到ON24并标记为已注册。 您可以将其他字段添加到表单，该信息将作为人员详细信息记录的一部分在Marketo中捕获。

>[!CAUTION]
>
>要成功集成，您必须使用Marketo表单注册事件人员，或使用具有正确API集成的非Marketo表单将注册数据推送到Marketo。

## 电子邮件和URL标记 {#emails-and-url-tokens}

使用Marketo创建邀请、确认、跟进和感谢电子邮件。

## Marketo确认电子邮件和URL标记 {#marketo-confirmation-email-and-url-token}

使用Marketo发送事件的确认电子邮件。 人员注册时，会收到一个用于输入事件的唯一URL。

>[!NOTE]
>
>要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌： `{{member.webinar url}}`. 当您发送确认URL时，此令牌会自动解析为人员的唯一确认URL。
>
>将确认电子邮件的类型设置为 **可操作** 确保注册用户收到其确认信息，即使他们已取消订阅。

>[!TIP]
>
>您可以配置ON24以发送确认、提醒或跟进电子邮件。 请参阅 [ON24帮助站点](https://www.on24.com/live-webcast-elite/){target="_blank"} 以了解更多信息。

## 注册子营销活动要求 {#registration-child-campaign-requirements}

事件包含一个或多个子营销策划，这些子营销策划可一起在项目状态中移动人员，并让您跟踪事件的效果。

子营销活动的示例包括邀请营销活动、注册营销活动和跟进营销活动。

>[!CAUTION]
>
>要使适配器完成其工作，您必须创建注册活动。 此营销活动必须由填写表单的人员触发，并且第一步必须将人员的项目状态更改为 **已注册**. 然后，营销策划会发送一封确认电子邮件。 有关详细信息，请参阅本文的其他部分。

**注册/确认（触发营销活动）**

* 智能列表
* 触发器依据 **填写表单**. 确保使用包含表单所在的登陆页面 **添加约束**，尤其是在多个登陆页面上使用相同表单时。

>[!CAUTION]
>
>您必须使用Marketo表单注册事件人员，或使用具有正确API集成的非Marketo表单将注册数据推送到Marketo。 这对于成功集成活动合作伙伴至关重要。

>[!NOTE]
>
>如果您在非Marketo登陆页面上使用Marketo表单，则您的触发器将为 **填写表单** 表单名称。

![](assets/image2015-12-22-15-3a20-3a51.png)

**流**

* **更改项目状态**  — 设置为网络研讨会 — >已注册。

在设置子营销活动时，此流程步骤是第一个流程步骤。 当人员的程序状态变为已注册时，Marketo会将注册信息推送到ON24。 没有其他状态会将该人员推倒。

* **发送电子邮件**  — 确认电子邮件。 将此电子邮件设置为 **可操作** 已注册的非订阅用户仍可接收该报文。

此 **发送电子邮件** 流程步骤必须是第二步。 确认电子邮件中包含 `{{member.webinar url}}`，其中填充了从ON24发回Marketo的信息。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>这些流程步骤的顺序非常重要，因为操作在Marketo中执行的顺序很重要。 此 **更改项目状态** 步骤将用户发送到ON24进行注册，并生成一个唯一的URL。 之后，您可以使用发送包含此唯一URL的确认电子邮件 `{{member.webinar URL}}` 令牌。
>
>如果返回人员时存在注册错误，他们将不会收到电子邮件确认。

您的下一步是 [测试ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [了解网络研讨会计划状态](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
