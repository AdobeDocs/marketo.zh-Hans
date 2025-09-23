---
description: 添加短信的流程步骤 — Marketo文档 — 产品文档
title: 为短信添加流程步骤
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 为短信添加流程步骤 {#add-a-flow-step-for-sms}

Marketo Engage有三个流程步骤可用于短信智能营销活动：

<table>
<tbody>
  <tr>
    <td style="width:25%">发送短信消息</td>
    <td>此流操作会将消息从Marketo智能列表中发送给订阅了用户选择加入的Vibes订阅列表的用户。 它不会启动订阅流程。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">了解详情</a>。</td>
  </tr>

<tr>
    <td style="width:25%">订阅体验列表</td>
    <td>此流程操作通过用户选择的Vibes客户获取促销活动启动短信订阅流程。 然后，Vibes发送确认消息，收件人必须在24小时内使用“Y”回复该消息以确认选择加入。 用户选择加入后，他们将成为关联的Vibes订阅列表的成员。</td>
  </tr>
  <tr>
    <td style="width:25%">取消订阅访客列表</td>
    <td>此流操作将从用户选择加入的Vibes订阅列表中取消订阅每个人。 当用户向您的代码发短信“STOP”时，其人员记录会更新，以反映他们不再是Vibes订阅列表的成员。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>发送短信消息时：
>
>* Marketo按电话号码进行重复数据删除。 因此，如果多人拥有相同的电话号码，则只有一人会收到消息，前提是他们仅属于一个Vibes订阅列表。 重复数据消除是在Vibes Subscription列表级别，而不是Marketo项目级别完成的。
>* Marketo不会发送给被列入阻止列表或营销暂停的人员。

有关设置流程步骤的一般信息，请参阅[将流程步骤添加到智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)。

以下是使用短信的基础知识。

1. 在“我的Marketo”中，单击&#x200B;**营销活动**。

   ![](assets/add-a-flow-step-for-sms-1.png)

1. 查找并选择要为其添加短信流的智能营销活动。

   屏幕快照

1. 在“智能列表”选项卡中，选择所需的触发器（例如“填写的表单”）。

   屏幕快照

1. 在&#x200B;**流**&#x200B;选项卡中，拖动到流步骤上（例如，**发送短信消息**）。 从下拉列表中选择短信消息和访客列表。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >“访客列表”选择器充当在智能列表中已标识的受众的后续过滤器，以仅定向属于该“访客”列表的潜在客户。
   >
   >**Subscribe to Vibes List**&#x200B;和&#x200B;**Unsubscribe from Vibes List**&#x200B;流具有不同的要求。 对于&#x200B;**订阅**，您必须选择Vibes列表和Vibes客户获取促销活动。 对于&#x200B;**取消订阅**，仅需要Vibes列表。
