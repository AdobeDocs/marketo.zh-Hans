---
unique-page-id: 7514918
description: 了解取消订阅 — Marketo文档 — 产品文档
title: 了解取消订阅
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 了解取消订阅 {#understanding-unsubscribe}

Marketo中实际上有几种不同类型的内置取消订阅。 它们都由人员对象上的字段表示，就像名字一样。

>[!NOTE]
>
>Marketo正在更改黑名单和白名单等术语，以便在我们的产阻止列表品中允许列表和。 在此更新过程中，您可能会在我们的UI和文档屏幕截图中看到旧术语，在我们的文档文本中看到新术语。 我们为任何混淆道歉。

所有这些字段都内置于您的Marketo订阅中。 它们都是布尔（复选框）类型。 它们可在Forms或 [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 流程步骤。

## 退订 {#unsubscribed}

该插件可在标准取消订阅页面上使用。 如果某人选中此框，或单击电子邮件中的取消订阅链接，他们将不再收到营销电子邮件。 但是，他们将获得 [操作电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## 营销暂停 {#marketing-suspended}

此字段由用户设置，用于将用户置于临时取消订阅状态。 只有在手动更改或使用更改数据值流步骤时，人员才能获得此状态。

## 电子邮件已暂停 {#email-suspended}

此状态会在发生硬退回后阻止某人发送24小时的邮件。 24小时后，该人将再次发邮件。

>[!NOTE]
>
>即使在24小时期限结束后，“电子邮件暂停”仍将保持选中状态，因此您可以指以前被标记为“已暂停”的人员。 要查看此人是否可邮寄，只需在电子邮件暂停后24小时计算即可。

## 列入阻止列表 {#blocklisted}

[这适用于像竞争对手一样的用户](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). 任何你想接收的人 **否** 电子邮件 — 运营、营销等。 他们什么也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
