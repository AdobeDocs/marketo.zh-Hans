---
description: 在智能营销活动中使用短信选项 — Marketo文档 — 产品文档
title: 在智能营销活动中使用短信选项
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 5c6e014224b33310c847c08784a70a08796d971a
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 在智能营销活动中使用短信选项 {#using-sms-options-in-a-smart-campaign}

在您之后 [创建短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message-2.md){target="_blank"}，您将需要在Smart Campaign中使用智能列表触发器和过滤器以获取好处。

>[!NOTE]
>
>如果您希望发送短信消息，我们提供 [特定文章](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md) 为了这个。

>[!PREREQUISITES]
>
>SMS触发器/过滤器仅在 [已启用访客服务](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## SMS触发器 {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

下面是一些示例：

此 **短信消息退回** 当短信消息退回时，触发器会启动流程，例如发送电子邮件。

此 **Vibes列表的订阅次数** 触发器会在人员订阅时启动流。

此 **点击短信消息中的链接** 当人员单击短信消息中的链接时，触发器将启动流程。

## 短信过滤器 {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

此 **订阅的访客列表** 筛选器查找具有 *从不* 订阅了Vibes。 这包括已取消订阅和已删除的人员，即使流程中会忽略已删除的人员。 此过滤器最适合报表。

相比之下， **Vibes列表的成员** 筛选器查找 _任何人_ 当前订阅了访客，最适合在智能营销活动或列表中使用。

>[!NOTE]
>
>所有短信过滤器都包含 **活动日期** 缺省情况下受约束。

## 短信流程步骤 {#sms-flow-steps}

有三个短信流程步骤可供选择。

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>发送短信消息</b></td>
    <td>此流操作会将消息从Marketo智能列表中发送给订阅了用户选择加入的Vibes订阅列表的用户。 它不会启动订阅流程。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">了解详情</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>订阅体验列表</b></td>
    <td>此流程操作通过用户选择的Vibes客户获取促销活动启动短信订阅流程。 然后，Vibes发送确认消息，收件人必须在24小时内使用“Y”回复该消息以确认选择加入。 用户选择加入后，他们将成为关联的Vibes订阅列表的成员。</td>
  </tr>
  <tr>
    <td style="width:20%"><b>取消订阅访客列表</b></td>
    <td>此流操作将从用户选择加入的Vibes订阅列表中取消订阅每个人。 当用户向您的代码发短信“STOP”时，其人员记录会更新，以反映他们不再是Vibes订阅列表的成员。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>此 **订阅体验列表** 和 **取消订阅访客列表** 流具有不同的要求。 对象 **订阅**&#x200B;中，您必须选择访客列表和访客获取促销活动。 对象 **取消订阅**，只需维贝斯列表。

>[!MORELIKETHIS]
>
>* [发送短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [为Smart Campaign定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [为Smart Campaign定义智能列表 |批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
