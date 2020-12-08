---
unique-page-id: 1147021
description: 更改所有者——营销文档——产品文档
title: 更改所有者
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# 更改所有者 {#change-owner}

如果已有人员已分配给某个所有者，您可以使用此流步骤将他们重新分配给另一个所有者。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用情况**

1. 只需选择您要更改到的所有者或潜在客户队列，即可开始！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允许将联系人分配到潜在客户队列。 对于SFDC联系人的记录：
   >
   >1. Marketo将仅在联系人同 **步到** Salesforce时创建重复潜在客户。 换言之，如果您使用“将人 **[员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** ”流步骤 `AssignTo=<a lead queue>`,Marketo将在Salesforce中创建重复潜在客户，并将其分配到潜在客户队列。
      >
      >
   2. 如果尝试在联系人 **上使用** “更改所有者流”步骤，则不会在Salesforce中创建重复。


   >[!NOTE]
   >
   >如果您的Salesforce帐户中尚不存在该记录，我们将同步该记录，然后将其分配给选定用户。
