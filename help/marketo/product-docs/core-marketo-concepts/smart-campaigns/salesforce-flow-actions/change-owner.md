---
unique-page-id: 1147021
description: 更改所有者 — Marketo文档 — 产品文档
title: 更改所有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
source-git-commit: 44c134811242b4136a3137cdd60e60edeb838c8c
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 更改所有者 {#change-owner}

如果您的现有人员已经分配给所有者，则可以使用此流程步骤将他们重新分配给其他所有者。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用情况**

1. 只需选择您要更改为的所有者或潜在客户队列，然后离开！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允许将联系人分配到潜在客户队列。 对于SFDC联系人的记录：
   >
   >1. Marketo将创建重复的潜在客户 **仅** 联系人同步到Salesforce时。 换句话说，如果您使用 **[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流量步骤 `AssignTo=<a lead queue>`,Marketo将在Salesforce中创建一个重复的潜在客户，并将其分配给潜在客户队列。
   >
   >1. 如果您使用 **更改所有者** 流程步骤中，Marketo会在Salesforce中创建一个重复的潜在客户。 要避免这种情况，请使用“SFDC类型”字段上的过滤器，该过滤器将操作限制为仅潜在客户。


   >[!NOTE]
   >
   >如果您的Salesforce帐户中尚不存在该记录，我们将同步该记录，然后将其分配给选定的用户。
