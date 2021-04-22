---
unique-page-id: 7515131
description: SFDC同步 — 删除潜在客户/联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 删除潜在客户/联系人
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同步：删除潜在客户/联系人{#sfdc-sync-deleting-a-lead-contact}

以下是一些详细信息：

* Marketo不会仅因Salesforce中删除了潜在客户而自动删除他人。 而是将字段“SFDC已删除”标志设置为true。 如果需要，可触发此字段以在Marketo中删除。
* [删除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 个性化操作。这将删除MKTO中的人员，但您也可以选择在`Salesforce`中删除。

* [从SFDCflow操](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) 作中删除：这将删除SFDC中的潜在客户，但您也可以选择删除Marketo中的人。
* 如果在Salesforce中删除了潜在客户(但在Marketo中未删除人员)，然后随后通过[与Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)同步流操作运行，则它将在Salesforce中创建新潜在客户。
