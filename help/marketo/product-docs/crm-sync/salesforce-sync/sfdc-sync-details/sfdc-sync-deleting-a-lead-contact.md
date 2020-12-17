---
unique-page-id: 7515131
description: SFDC同步——删除潜在客户／联系人- Marketo文档——产品文档
title: SFDC同步——删除潜在客户／联系人
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# SFDC同步：删除潜在客户／联系人{#sfdc-sync-deleting-a-lead-contact}

下面是一些详细信息：

* Marketo不会仅因Salesforce中删除了潜在客户而自动删除人员。 而是将字段“SFDC已删除”标志设置为true。 如果需要，您可以触发此字段在Marketo中删除。
* [删除](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 个人流操作。这将删除MKTO中的人员，但您也可以选择在`Salesforce`中删除。

* [从SFDCflow操](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) 作中删除：这将删除SFDC中的潜在客户，但您也可以选择删除Marketo中的人员。
* 如果Salesforce中删除了潜在客户（但Marketo中未删除人员），随后通过[与Salesforce同步](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)流动操作运行，则它将在Salesforce中创建新潜在客户。

换句话说，它像魔法一样工作！

![—](assets/image2015-5-20-15-3a3-3a27.png)

