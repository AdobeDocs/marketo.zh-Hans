---
unique-page-id: 7515131
description: SFDC同步 — 删除潜在客户/联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 删除潜在客户/联系人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# SFDC同步：删除潜在客户/联系人 {#sfdc-sync-deleting-a-lead-contact}

以下是一些详细信息：

* Marketo不会仅仅因为潜在客户已在Salesforce中删除而自动删除人员。 而是字段“SFDC已删除”标志设置为true。 如果需要，您可以在Marketo中触发要删除的此字段。
* [删除人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) flow操作。 这将删除MKTO中的人员，但您可以选择删除 `Salesforce` 也是。

* [从SFDC中删除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) flow action：这将删除SFDC中的潜在客户，但您也可以选择删除Marketo中的人员。
* 如果潜在客户在Salesforce中被删除(但人员未在Marketo中被删除)，然后会运行 [与Salesforce同步](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) flow action之后，它将在Salesforce中创建一个新商机。
