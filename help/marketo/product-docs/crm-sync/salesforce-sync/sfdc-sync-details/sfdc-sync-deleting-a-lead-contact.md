---
unique-page-id: 7515131
description: SFDC同步——删除潜在客户／联系人- Marketo文档——产品文档
title: SFDC同步——删除潜在客户／联系人
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# SFDC同步：删除潜在客户／联系人 {#sfdc-sync-deleting-a-lead-contact}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

下面是一些详细信息：

* Marketo不会仅因Salesforce中删除了潜在客户而自动删除人员。 而是将字段“SFDC已删除”标志设置为true。 如果需要，您可以触发此字段在Marketo中删除。
* [删除人员流](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) (Person Flow)操作。 这将删除MKTO中的人员，但您也可以选择删除 `Salesforce` 人员。

* [从SFDC流操作](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) “删除”:这将删除SFDC中的潜在客户，但您也可以选择删除Marketo中的人员。
* 如果Salesforce中删除了潜在客户（但Marketo中未删除人员），随后通过与Salesforce [同步流动操作](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) ，则它将在Salesforce中创建新潜在客户。

换句话说，它像魔法一样工作！

![--](assets/image2015-5-20-15-3a3-3a27.png)

