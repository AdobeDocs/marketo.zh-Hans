---
unique-page-id: 11378871
description: 在智能列表触发器和过滤器中使用查看SMS消息 — Marketo Docs — 产品文档
title: 在智能列表触发器和过滤器中使用视频短信
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---


# 在智能列表触发器和过滤器{#use-vibes-sms-messages-in-smart-list-triggers-and-filters}中使用查看SMS消息

在[创建Vibes SMS消息](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)后，您将希望在智能活动中使用智能列表触发器和过滤器，以获得优势。 下面介绍如何操作。

1. 在“我的营销人员”中，单击&#x200B;**营销活动**。

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. 选择您要在其中使用SMS资源的智能活动。 在触发器上拖动，如常用的&#x200B;**填充表单**。

   ![](assets/fills-out-form-pull-over.jpg)

## SMS触发器{#sms-triggers}

还有其他SMS触发器可用。 SMS触发器仅在启用Vibes服务时才显示。

![](assets/new-sms-search2.png)

以下是几个示例：

SMS消息弹回触发器启动一个流，如在SMS消息弹回时发送电子邮件。

![](assets/sms-message-bounces-real.jpg)

**订阅Vibes列表**&#x200B;触发器在用户订阅时启动流。

![](assets/subscribes-to-vibes-list-real.jpg)

当用户单击SMS消息中的链接时，SMS消息&#x200B;**中的**&#x200B;单击链接触发将启动流。

![](assets/clicks-link-in-sms-message.jpg)

## SMS过滤器{#sms-filters}

您还可以在智能列表中使用Vibes过滤器。 **订阅Vibes列表**&#x200B;筛选器可查找具有&#x200B;*曾订阅Vibes的*&#x200B;的任何人。 这包括未订阅和已删除的人员，即使从流中忽略已删除的人员。 此滤镜最适合报告。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

相比之下，Vibes 列表&#x200B;**的**&#x200B;成员会查找当前订阅Vibes的&#x200B;_任何_，最适合在智能活动或列表中使用。

![](assets/image001.png)

>[!NOTE]
>
>默认情况下，所有SMS过滤器都包含活动&#x200B;**约束的**&#x200B;日期。

在智能列表中设置Vibes触发器和过滤器后，您可以[定义流](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md)。

>[!MORELIKETHIS]
>
>* [为智能列表定义智能活动 |触发器](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [查找过滤器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

