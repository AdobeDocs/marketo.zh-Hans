---
unique-page-id: 7514918
description: 了解取消订阅 — Marketo文档 — 产品文档
title: 了解取消订阅
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 了解取消订阅 {#understanding-unsubscribe}

Marketo中实际上有多种不同类型的内置取消订阅。 它们都由person对象上的字段表示，就像名字一样。

>[!NOTE]
>
>Marketo正在将黑名单和白名单等术语更改为产品中的阻止列表允许列表和。 在本次更新中，您可能会在UI和文档屏幕截图中看到旧术语，并在文档文本中看到新术语。 造成任何混淆，我们深表歉意。

所有这些字段均内置到您的Marketo订阅中。 它们都是布尔型（复选框）类型。 它们可以在Forms中使用，或者 [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 流程步骤。

## 退订 {#unsubscribed}

该选项在标准取消订阅页面上使用。 如果人员选中此框，或单击电子邮件中的取消订阅链接，他们将不再收到营销电子邮件。 然而，他们将获得 [操作电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## 营销暂停 {#marketing-suspended}

该字段由用户设置，用于临时取消订阅用户。 仅当手动更改人员或使用更改数据值流程步骤时，他们才能获得此状态。

## 电子邮件已暂停 {#email-suspended}

此状态会在发生硬退回后24小时内阻止人员发送邮件。 24小时后，该用户将再次变为可邮寄状态。

>[!NOTE]
>
>即使24小时期限结束后，电子邮件暂停仍会保持选中状态，因此您可以引用历来标记为此类的人员。 要查看此人是否可邮件，只需在电子邮件暂停后24小时内计算即可。

## 已列入阻止列表 {#blocklisted}

[将其用于竞争对手等人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). 您希望接收的任何人 **否** 电子邮件 — 运营、营销等。 他们什么也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
