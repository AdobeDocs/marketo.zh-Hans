---
description: 添加短信的流程步骤 — Marketo文档 — 产品文档
title: 为短信添加流程步骤
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 为短信添加流程步骤 {#add-a-flow-step-for-sms}

Marketo Engage包含三个流程步骤，您可以在短信智能营销活动中使用：

* **发送短信消息**  — 此流操作将消息从Marketo智能列表发送给订阅了用户选择加入的Vibes订阅列表的用户。 它不会启动订阅流程。
* **订阅体验列表**  — 此流程操作通过用户选择的Vibes客户获取促销活动启动短信订阅流程。 然后，Vibes发送确认消息；收件人必须回复“Y”才能在24小时内确认选择加入。 用户选择加入后，他们将成为关联的Vibes订阅列表的成员。
* **取消订阅访客列表**  — 此流操作将从用户选择加入的Vibes订阅列表中取消订阅每个人。 当用户向您的代码发送文本“停止”时，其人员记录将更新，以反映他们不再是Vibes订阅列表的成员。

>[!NOTE]
>
>发送短信消息时：
>
>* Marketo按电话号码进行重复数据删除。 因此，如果多人拥有相同的电话号码，则只有一人会收到消息，前提是他们仅属于一个Vibes订阅列表。 重复数据消除是在Vibes Subscription列表级别，而不是Marketo项目级别完成的。
>* Marketo不会发送给被列入阻止列表或营销暂停的人员。

有关设置流程步骤的一般信息，请参阅 [向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

以下是使用短信的基础知识。

1. 在“我的Marketo”中，单击 **营销活动**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. 查找并选择要为其添加短信流的智能营销活动。

   屏幕快照

1. 在“智能列表”选项卡中，选择所需的触发器（例如“填写的表单”）。

   屏幕快照

1. 在 **流量** 选项卡，在流程步骤上拖动(例如， **发送短信消息**)。 从下拉列表中选择短信消息和访客列表。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >“访客列表”选择器充当在智能列表中已标识的受众的后续过滤器，以仅定向属于该“访客”列表的潜在客户。
   >
   >此 **订阅体验列表** 和 **取消订阅访客列表** 流具有不同的要求。 对象 **订阅**&#x200B;中，您必须选择访客列表和访客获取促销活动。 对象 **取消订阅**，只需维贝斯列表。
