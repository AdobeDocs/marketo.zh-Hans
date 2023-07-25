---
unique-page-id: 11379045
description: 添加短信的流程步骤 — Marketo文档 — 产品文档
title: 为短信添加流程步骤
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 为短信添加流程步骤 {#add-a-flow-step-for-sms}

Marketo有三个流程步骤，您可以在短信智能营销活动中使用：

* **发送短信消息**  — 此流操作将消息从Marketo智能列表中发送给订阅了用户选择的Vibes订阅列表的用户。 它不会启动订阅过程。
* **订阅振动列表**  — 此流程操作通过用户选择的Vibes客户获取促销活动启动短信订阅流程。 然后，Vibes发送确认消息；收件人必须回复该消息才能完成订阅过程。
* **取消订阅Vibes列表**  — 此流操作从用户选择的Vibes订阅列表中取消订阅每个人。

>[!NOTE]
>
>发送短信消息时：
>
>* Marketo按电话号码进行重复数据删除。 因此，如果多个用户拥有相同的电话号码，则只有一个用户会收到该消息。
>* Marketo不会发送给被列入阻止列表或营销活动被暂停的人员。

有关设置流步骤的一般信息，请参阅 [向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

以下是使用短信的基础知识。

1. 在“我的Marketo”中，单击 **营销活动**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. 查找要将短信流添加到的智能营销活动。 单击 **流量** 选项卡。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. 拖动流的上方，例如， **发送短信消息**. 从下拉列表中选择短信消息和振动列表。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >“Vibes List”选择器对智能列表中已识别的受众起到进一步过滤的作用，以仅定向属于该Vibes列表的潜在客户。
   >
   >此 **订阅振动列表** 和 **取消订阅Vibes列表** 流具有不同的要求。 对象 **订阅**&#x200B;中，您必须选择多维数据集列表和多维数据集客户获取营销活动。 对象 **取消订阅**，只需振动列表。
