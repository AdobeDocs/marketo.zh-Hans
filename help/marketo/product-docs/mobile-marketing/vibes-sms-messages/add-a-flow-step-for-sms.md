---
unique-page-id: 11379045
description: 为短信添加流程步骤 — Marketo文档 — 产品文档
title: 为短信添加流程步骤
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 为短信添加流程步骤 {#add-a-flow-step-for-sms}

Marketo有三个流程步骤，可在短信智能营销活动中使用：

* **发送短信消息**  — 此流动操作向订阅用户选择的Vibes订阅列表的Marketo智能列表用户发送消息。 它不会启动订阅过程。
* **订阅Vibes列表**  — 此流程操作通过用户选择的访问客户获取促销活动，启动短信订阅流程。 然后，访客会发送确认消息；收件人必须回复它才能完成订阅过程。
* **取消订阅Vibes列表**  — 此流量操作将从用户选择的Vibes订阅列表中取消每个人的订阅。

>[!NOTE]
>
>发送短信消息时：
>
>* Marketo按电话号码去重复。 因此，如果多个人拥有相同的电话号码，则只有一个人会收到该消息。
>* Marketo不会发送给被或营销列入阻止列表暂停的人员。


有关设置流程步骤的一般信息，请参阅 [向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

以下是使用短信的基础知识。

1. 在我的Marketo中，单击 **营销活动**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. 查找要将短信流添加到的智能营销活动。 单击 **流量** 选项卡。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 例如，在流量上拖动 **发送短信消息**. 从下拉列表中选择短信消息和视频列表。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >“可视化列表”选择器可作为对智能列表中已识别受众的进一步过滤器，以仅定位属于该可视化列表的那些潜在客户。
   >
   >的 **订阅Vibes列表** 和 **取消订阅Vibes列表** 流有不同的要求。 对于 **订阅**，则必须选择“访客”列表和“访客获取”营销活动。 对于 **取消订阅**，则仅需要“访客”列表。
