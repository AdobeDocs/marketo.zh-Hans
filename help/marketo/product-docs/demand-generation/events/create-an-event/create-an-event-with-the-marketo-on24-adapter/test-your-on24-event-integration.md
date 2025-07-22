---
unique-page-id: 10096677
description: 测试ON24事件集成 — Marketo文档 — 产品文档
title: 测试ON24事件集成
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 测试ON24事件集成 {#test-your-on-event-integration}

确保彻底测试您的事件集成。

## 运行第一个活动之前的建议测试序列 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填写事件的注册表，并使用有效的电子邮件地址进行测试。
1. 确认在Marketo事件的成员资格网格中显示状态为&#x200B;**已注册**&#x200B;的测试名称。
1. 确认测试名称在ON24中还显示为&#x200B;**已注册**。
1. 确认您用于注册测试名称的有效电子邮件地址收到一封确认电子邮件，告知事件并且唯一URL已在电子邮件中解析。

   >[!NOTE]
   >
   >您必须在确认电子邮件中使用`{{member.webinar url}}`令牌，以便在每个注册人的电子邮件中显示唯一URL。

## 活动后 {#after-the-event}

以下是事件发生后数据更新的方式：

* Marketo每晚从ON24检索与会者数据。
* 在与会者数据在Marketo和ON24之间同步后，Marketo将成员资格状态更新为[!UICONTROL Attended]、[!UICONTROL Attended On-demand]或[!UICONTROL No Show]。 在事件的&#x200B;**[!UICONTROL Summary]**&#x200B;选项卡中，事件状态更新为&#x200B;**[!UICONTROL Event Complete]**。

>[!MORELIKETHIS]
>
>* [ON24事件集成示例](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [了解Marketo ON24适配器事件](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
