---
unique-page-id: 10096675
description: 创建子营销活动和本地资产 — Marketo文档 — 产品文档
title: 创建子营销活动和本地资产
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 1%

---

# 创建子营销活动和本地资产 {#create-child-campaigns-and-local-assets}

使用Design Studio创建子营销活动和本地资产。

## 登陆页面和表单 {#landing-page-and-form}

要确保用户在ON24中正确注册，您的Marketo表单中必须包含以下字段：

* 名
* 姓
* 电子邮件地址

您还可以将以下字段推送到ON24:

* 公司名称
* 职务

通过向注册营销活动添加正确的流程步骤，人员将被推送到ON24并标记为已注册。 您可以向表单中添加其他字段，该信息将作为人员详细信息记录的一部分在Marketo中捕获。

>[!CAUTION]
>
>要成功集成，您必须使用Marketo表单为活动注册人员，或使用正确的API集成的非Marketo表单将注册数据推送到Marketo。

## 电子邮件和URL令牌 {#emails-and-url-tokens}

使用Marketo创建邀请、确认、跟进和感谢电子邮件。

## Marketo确认电子邮件和URL令牌 {#marketo-confirmation-email-and-url-token}

使用Marketo发出事件的确认电子邮件。 当人员进行注册时，他/她会收到用于输入事件的唯一URL。

>[!NOTE]
>
>要使用此唯一URL填充确认电子邮件，请在电子邮件中使用以下令牌： `{{member.webinar url}}`. 当您发出确认URL时，此令牌会自动解析为人员的唯一确认URL。
>
>将确认电子邮件的类型设置为 **运行** 确保注册人员即使被取消订阅，也会收到其确认信息。

>[!TIP]
>
>您可以配置ON24以发出确认、提醒或跟进电子邮件。 请参阅 [ON24帮助网站](https://www.on24.com/live-webcast-elite/){target=&quot;_blank&quot;}以了解详细信息。

## 注册子营销活动要求 {#registration-child-campaign-requirements}

事件包含一个或多个子营销活动，所有这些营销活动都可协同工作，以便让人员浏览项目状态，并让您跟踪事件的效果。

子营销活动的示例包括邀请营销活动、注册营销活动和后续营销活动。

>[!CAUTION]
>
>要使适配器完成其工作，必须创建注册营销活动。 此营销活动必须由填写表单的人员触发，并且第一步必须将人员的项目状态更改为 **已注册**. 然后，营销活动会发送确认电子邮件。 有关详细信息，请参阅本文的其余部分。

**注册/确认（触发营销活动）**

* 智能列表
* 触发器基于 **填写表单**. 请务必使用 **添加约束**，尤其是当同一表单用于多个登陆页面时。

>[!CAUTION]
>
>您必须使用Marketo表单为活动注册人员，或使用正确API集成的非Marketo表单将注册数据推送到Marketo。 这对于活动合作伙伴集成的成功至关重要。

>[!NOTE]
>
>如果您在非Marketo登陆页面上使用Marketo表单，则触发器将为 **填写表单** ，其中包含“表单名称”。

![](assets/image2015-12-22-15-3a20-3a51.png)

**流量**

* **更改程序状态**  — 设置为网络研讨会 — >已注册。

在设置子营销活动时，此流程步骤是第一个流程步骤。 当某人的项目状态变为“已注册”时，Marketo会将注册信息推送到ON24。 没有其他状态会将人推过去。

* **发送电子邮件**  — 确认电子邮件。 将此电子邮件设置为 **运行** 这样注册的未注册用户仍然能收到它。

的 **发送电子邮件** 流程步骤必须是第二步。 确认电子邮件包含 `{{member.webinar url}}`，其中填充了从ON24发送回Marketo的信息。

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>由于操作在Marketo中的执行顺序，因此这些流程步骤的顺序非常重要。 的 **更改程序状态** 步骤会将人员发送到ON24进行注册，并生成一个唯一的URL。 发生此情况后，您可以使用 `{{member.webinar URL}}` 令牌。
>
>如果返回人员时出现注册错误，则他们将不会收到电子邮件确认。

下一步是 [测试ON24事件集成](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}。

>[!MORELIKETHIS]
>
>* [了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}
>* [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
>* [了解网络研讨会计划状态](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}

