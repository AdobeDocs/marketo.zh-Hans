---
unique-page-id: 7514918
description: 了解取消订阅 — Marketo文档 — 产品文档
title: 了解取消订阅
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 1%

---

# 了解取消订阅 {#understanding-unsubscribe}

Marketo中实际上有多种不同类型的内置取消订阅。 它们全部由人员对象上的字段表示，就像“名字”一样。

所有这些字段均内置到您的Marketo订阅中。 它们是布尔型（复选框）类型。 它们可以在Forms或[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)流程步骤中使用。

## 退订 {#unsubscribed}

该选项在标准取消订阅页面上使用。 如果人员选中此框，或单击电子邮件中的取消订阅链接，则将不再接收营销电子邮件。 但是，他们将收到[操作电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

## 营销暂停 {#marketing-suspended}

该字段由用户设置，用于临时取消订阅用户。 仅当手动更改人员或使用更改数据值流程步骤时，他们才能获得此状态。

## 电子邮件已暂停 {#email-suspended}

硬退回后，此状态在24小时内阻止人员发送邮件。 24小时后，该用户将再次变为邮寄。

>[!NOTE]
>
>即使24小时期限结束后，已暂停的电子邮件仍会保持选中状态，以便您可以引用历来已将此电子邮件标记为已暂停的人员。 要查看此人是否可邮寄，只需在电子邮件暂停后24小时内计算即可。

## 已列入阻止列表 {#blocklisted}

[将此用于竞争对手等人](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。 您希望接收&#x200B;**no**&#x200B;电子邮件的任何人 — 运营、营销等。 他们什么也得不到！

![](assets/image2015-5-18-12-3a6-3a40.png)
