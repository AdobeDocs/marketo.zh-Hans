---
unique-page-id: 7514918
description: 了解取消订阅- Marketo Docs —— 产品文档
title: 了解取消订阅
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 了解取消订阅{#understanding-unsubscribe}

Marketo中实际上有几种不同类型的内置取消订阅。 它们都由person对象上的字段表示，就像“名字”一样。

>[!NOTE]
>
>Marketo正在更改黑名单和白名单等术语，以在我们的产阻止列表品中进允许列表行和。 在此更新过程中，您可能会在我们的UI和文档屏幕截图中看到旧条款，在我们的文档文本中看到新条款。 我们为任何混淆表示歉意。

所有这些字段都内置于您的Marketo订阅。 它们都是布尔（复选框）类型。 它们可以在Forms或[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)流步骤中使用。

## 取消订阅{#unsubscribed}

此选项用于标准取消订阅页面。 如果某人选中此框或单击电子邮件中的取消订阅链接，他们将不再收到营销电子邮件。 但是，他们将收到[操作电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

## 已暂停营销{#marketing-suspended}

此字段由用户设置，用于将用户置于临时取消订阅状态。 只有在手动更改或使用更改数据值流步骤时，才能达到此状态。

## 电子邮件已挂起{#email-suspended}

在出现硬弹回后，此状态会阻止某人发送24小时的邮件。 24小时后，该人将可再次发邮件。

>[!NOTE]
>
>即使在24小时内暂停电子邮件也将保持选中状态，因此您可以指的是以前被标记为此类的用户。 要查看此人是否可发送邮件，只需在电子邮件暂停后24小时计算。

## 列入阻止列表 {#blocklisted}

[将它用于竞争对手等人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。希望收到&#x200B;**不**&#x200B;电子邮件的任何人，包括运营、营销等。 他们什么也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
