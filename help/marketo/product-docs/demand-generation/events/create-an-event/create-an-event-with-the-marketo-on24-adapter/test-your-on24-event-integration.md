---
unique-page-id: 10096677
description: 测试ON24事件集成 — Marketo文档 — 产品文档
title: 测试ON24事件集成
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# 测试ON24事件集成 {#test-your-on-event-integration}

确保彻底测试您的事件集成。

## 运行第一个活动之前建议的测试序列 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填写事件的注册表，并使用有效的电子邮件地址进行测试。
1. 确认显示的测试名称包含 **已注册** Marketo事件的成员资格网格中的状态。
1. 确认测试名称还显示为 **已注册** 在ON24中。
1. 确认您用于注册测试名称的有效电子邮件地址收到了一封发送给事件的确认电子邮件，并且唯一URL已在电子邮件中解析。

   >[!NOTE]
   >
   >您必须使用 `{{member.webinar url}}` 确认电子邮件中的令牌，以便在每位注册人的电子邮件中显示唯一的URL。

## 在事件之后 {#after-the-event}

以下是事件发生后数据更新的方式：

* Marketo每晚从ON24检索出席者数据。
* 在与会者数据在Marketo和ON24之间同步后，Marketo会将会员资格状态更新为“已参加”、“已参加”、“按需”或“无显示”。 在事件的 **摘要** 选项卡中，事件状态将更新为 **事件结束**.

>[!MORELIKETHIS]
>
>* [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
