---
description: 在智能营销活动中使用短信选项 — Marketo文档 — 产品文档
title: 在智能营销活动中使用短信选项
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 3%

---

# 在智能营销活动中使用短信选项 {#using-sms-options-in-a-smart-campaign}

在您[创建SMS消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}后，您将需要在智能营销活动中使用智能列表触发器和过滤器以获取优势。

>[!NOTE]
>
>如果您希望发送短信消息，我们针对此内容发表了[特定文章](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}。

>[!PREREQUISITES]
>
>仅当[Vibes服务已启用](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}时，才会显示SMS触发器/过滤器。

## SMS触发器 {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

下面是一些示例：

**SMS消息退回**&#x200B;触发器会在短信消息退回时启动流程，例如发送电子邮件。

**Subscripts to Vibes List**&#x200B;触发器会在人员订阅时启动流。

当某人单击短信消息中的链接时，**点击短信消息中的链接**&#x200B;触发器将启动流程。

## 短信过滤器 {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

**订阅的Vibes列表**&#x200B;筛选器查找&#x200B;*ever*&#x200B;订阅了Vibes的任何人。 这包括已取消订阅和已删除的人员，即使流程中会忽略已删除的人员。 此过滤器最适合报表。

相反，**Vibes列表的成员**&#x200B;筛选器将查找当前订阅了Vibes的&#x200B;*任何人*，该筛选器最适合于在智能营销活动或列表中使用。

>[!NOTE]
>
>默认情况下，所有SMS筛选器都包含&#x200B;**活动日期**&#x200B;约束。

## 短信流程步骤 {#sms-flow-steps}

有三个短信流程步骤可供选择。

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>发送短信消息</b></td>
    <td>此流操作会将消息从Marketo智能列表中发送给订阅了用户选择加入的Vibes订阅列表的用户。 它不会启动订阅流程。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">了解详情</a>。</td>
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
>**Subscribe to Vibes List**&#x200B;和&#x200B;**Unsubscribe from Vibes List**&#x200B;流具有不同的要求。 对于&#x200B;**订阅**，您必须选择Vibes列表和Vibes客户获取促销活动。 对于&#x200B;**取消订阅**，仅需要Vibes列表。

>[!MORELIKETHIS]
>
>* [发送短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [为智能营销活动定义智能列表 | 触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [为智能营销活动定义智能列表 | 批次](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
