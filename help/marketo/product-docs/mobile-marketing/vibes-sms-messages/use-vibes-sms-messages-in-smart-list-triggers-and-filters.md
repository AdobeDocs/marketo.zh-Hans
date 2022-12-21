---
unique-page-id: 11378871
description: 在智能列表触发器和过滤器中使用查看的短信消息 — Marketo文档 — 产品文档
title: 在智能列表触发器和过滤器中使用视频短信消息
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# 在智能列表触发器和过滤器中使用视频短信消息 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

在 [创建视频短信消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)，则您将需要在智能营销活动中使用智能列表触发器和过滤器，以获得好处。 这是方法。

1. 在我的Marketo中，单击 **营销活动**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. 选择要在其中使用短信资产的智能营销活动。 将鼠标拖到触发器上，例如 **填写表单**.

   ![](assets/fills-out-form-pull-over.jpg)

## 短信触发器 {#sms-triggers}

还有其他一些短信触发器可用。 短信触发器仅在启用了视频服务时才显示。

![](assets/new-sms-search2.png)

以下是一些示例：

短信消息退回触发器会在短信消息退回时启动一个流程，例如发送电子邮件。

![](assets/sms-message-bounces-real.jpg)

的 **访客列表订阅** 当人员订阅时，触发器会启动流程。

![](assets/subscribes-to-vibes-list-real.jpg)

的 **短信消息中的点击链接** 当用户单击短信消息中的链接时，触发器会启动一个流程。

![](assets/clicks-link-in-sms-message.jpg)

## 短信过滤器 {#sms-filters}

您还可以在智能列表中使用可视化过滤器。 的 **订阅了Vibes列表** 过滤器会查找 *ever* 订阅了维比斯。 这包括已取消订阅和已删除的人员，即使流程中已删除的人员被忽略也是如此。 此过滤器最适合于报表。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

相比之下， **Vibes列表成员** 过滤器查找 _任何人_ 当前已订阅Vibes，最适合在智能促销活动或列表中使用。

![](assets/image001.png)

>[!NOTE]
>
>所有短信过滤器都包括 **活动日期** 约束。

在智能列表中设置Vibe触发器和过滤器后，您可以 [定义流量](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [为智能营销活动定义智能列表 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [查找过滤器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

