---
unique-page-id: 10096677
description: 测试ON24事件集成- Marketo Docs —— 产品文档
title: 测试ON24事件集成
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# 测试ON24事件集成 {#test-your-on-event-integration}

确保彻底测试事件集成。

## 运行第一个活动前推荐的测试序列 {#recommended-test-sequence-before-running-your-first-campaign}

1. 填写事件的注册表，并使用有效的电子邮件地址进行测试。
1. 确认测试名称在Marketo事件 **的** “会员资格”网格中显示为“已注册”状态。
1. 确认测试名称在ON24中也 **显示为** “Registered”。
1. 确认您用于注册测试名称的有效电子邮件地址已收到一封确认电子邮件给事件，且该唯一URL已在电子邮件中解析。

   >[!NOTE]
   >
   >您必须在确认 `{{member.webinar url}}` 电子邮件中使用令牌，才能在每个注册者的电子邮件中显示唯一的URL。

## 事件 {#after-the-event}

以下是事件发生后数据的更新方式：

* Marketo每晚从ON24检索与会者数据。
* 在Marketo和ON24之间同步与会者数据后，Marketo会将会员资格状态更新为“已出席”、“已出席点播”或“无显示”。 在事件的“摘 **要** ”选项卡中，事件状态将更新为 **“事件完成”**。

>[!NOTE]
>
>**相关文章**
>
>* [示例ON24事件集成](example-on24-event-integration.md)
>* [了解ON24适配器的营销事件](understanding-marketo-on24-adapter-events.md)

>



