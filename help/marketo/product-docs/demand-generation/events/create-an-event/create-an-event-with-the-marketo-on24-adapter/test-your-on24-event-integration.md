---
unique-page-id: 10096677
description: 测试ON24事件集成 — Marketo文档 — 产品文档
title: 测试ON24事件集成
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 测试ON24事件集成 {#test-your-on-event-integration}

>[!IMPORTANT]
>
>自2022年8月起，ON24不再支持新的Marketo集成。 本文中的信息仅适用于现有用户。

确保对事件集成进行彻底测试。

## 运行第一个营销活动之前推荐的测试序列 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填写活动的注册表，并使用有效的电子邮件地址进行测试。
1. 使用 **已注册** 状态。
1. 确认测试名称也显示为 **已注册** 在ON24中。
1. 确认用于注册测试名称的有效电子邮件地址已收到一封确认电子邮件，发送给该事件，并且该唯一URL已在电子邮件中解析。

   >[!NOTE]
   >
   >您必须使用 `{{member.webinar url}}` 令牌，以便在每个注册者的电子邮件中显示唯一URL。

## 事件之后 {#after-the-event}

以下是事件发生后数据的更新方式：

* Marketo每晚从ON24中检索与会者数据。
* 在Marketo与ON24之间同步与会者数据后，Marketo会将会员状态更新为“已出席”、“已出席（按需）”或“无节目”。 在 **概要** 选项卡，事件状态将更新为 **事件结束**.

>[!MORELIKETHIS]
>
>* [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

