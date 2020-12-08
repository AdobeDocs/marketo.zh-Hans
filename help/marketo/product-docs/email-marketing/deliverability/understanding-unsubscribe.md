---
unique-page-id: 7514918
description: 了解取消订阅- Marketo Docs —— 产品文档
title: 了解取消订阅
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 了解取消订阅 {#understanding-unsubscribe}

Marketo中实际上有几种不同类型的内置取消订阅。 它们都由person对象上的字段表示，就像“名字”一样。

>[!NOTE]
>
>Marketo正在更改黑名单和白名单等术语，以在我们的产阻止列表品中进允许列表行和。 在此更新过程中，您可能会在我们的UI和文档屏幕截图中看到旧条款，在我们的文档文本中看到新条款。 我们为任何混淆表示歉意。

所有这些字段都内置于您的Marketo订阅。 它们都是布尔（复选框）类型。 它们可用于Forms或 [更改数据值](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 流步骤。

## 取消订阅 {#unsubscribed}

此选项用于标准取消订阅页面。 如果某人选中此框或单击电子邮件中的取消订阅链接，他们将不再收到营销电子邮件。 不过，他们会收到运营电 [子邮件](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

## 营销已暂停 {#marketing-suspended}

此字段由用户设置，用于将用户置于临时取消订阅状态。 只有在手动更改或使用更改数据值流步骤时，才能达到此状态。

## 电子邮件已暂停 {#email-suspended}

在出现硬弹回后，此状态会阻止某人发送24小时的邮件。 24小时后，该人将可再次发邮件。

>[!NOTE]
>
>即使在24小时内暂停电子邮件也将保持选中状态，因此您可以指的是以前被标记为此类的用户。 要查看此人是否可发送邮件，只需在电子邮件暂停后24小时计算。

## 列入阻止列表 {#blocklisted}

[将它用于竞争对手等人](http://docs.marketo.com/x/uwOQ)。 任何您希望不接 **收电** 子邮件的人，如运营、营销等。 他们什么也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)

