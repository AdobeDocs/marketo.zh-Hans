---
description: 在智能列表触发器和过滤器中使用短信选项 — Marketo文档 — 产品文档
title: 在智能列表触发器和过滤器中使用短信选项
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 在智能列表触发器和过滤器中使用短信选项 {#use-sms-options-in-smart-list-triggers-and-filters}

新建文档

在您之后 [创建短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}，您将需要在Smart Campaign中使用智能列表触发器和过滤器以获取好处。

>[!PREREQUISITES]
>
>SMS触发器/过滤器仅在 [已启用访客服务](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## SMS触发器 {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

下面是一些示例：

此 **短信消息退回** 当短信消息退回时，触发器会启动流程，例如发送电子邮件。

此 **Vibes列表的订阅次数** 触发器会在人员订阅时启动流。

此 **点击短信消息中的链接** 当人员单击短信消息中的链接时，触发器将启动流程。

## 短信过滤器 {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

您还可以在智能列表中使用维客筛选器。 此 **订阅的访客列表** 筛选器查找具有 *从不* 订阅了Vibes。 这包括已取消订阅和已删除的人员，即使流程中会忽略已删除的人员。 此过滤器最适合报表。

相比之下， **Vibes列表的成员** 筛选器查找 _任何人_ 当前订阅了访客，最适合在智能营销活动或列表中使用。

>[!NOTE]
>
>所有短信过滤器都包含 **活动日期** 缺省情况下受约束。

在智能列表中设置Vibes触发器和过滤器后，您可以 [定义流](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [发送短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [为Smart Campaign定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [查找筛选器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
