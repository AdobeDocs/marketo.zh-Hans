---
unique-page-id: 7515131
description: SFDC同步 — 删除潜在客户/联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 删除潜在客户/联系人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同步：删除潜在客户/联系人 {#sfdc-sync-deleting-a-lead-contact}

以下是一些详细信息：

* Marketo不会仅因为Salesforce中删除了潜在客户而自动删除人员。 字段“SFDC已删除”标记设置为true。 如果需要，您可以触发此字段以在Marketo中删除。
* [删除人员](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 流量操作。 这会删除MKTO中的人员，但您可以选择在 `Salesforce` 也是。

* [从SFDC中删除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) 流量操作：这会删除SFDC中的潜在客户，但您也可以选择删除Marketo中的人员。
* 如果在Salesforce中删除了潜在客户(但在Marketo中未删除人员)，然后在 [与Salesforce同步](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) 流程操作，则会在Salesforce中创建新潜在客户。
