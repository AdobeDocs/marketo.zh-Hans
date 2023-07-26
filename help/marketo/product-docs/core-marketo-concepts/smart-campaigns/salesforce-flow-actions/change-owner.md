---
unique-page-id: 1147021
description: 更改所有者 — Marketo文档 — 产品文档
title: 更改所有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# 更改所有者 {#change-owner}

如果您现有的人员已分配给所有者，则可以使用此流程步骤将它们重新分配给其他所有者。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用情况**

1. 只需选择所有者或您要更改为的潜在客户队列即可开始！

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce不允许将联系人分配给潜在客户队列。 对于SFDC联系人记录：
   >
   >1. Marketo将创建一个重复的潜在客户 **仅限** 联系人同步到Salesforce时。 换言之，如果您使用 **[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** 流程步骤和 `AssignTo=<a lead queue>`，Marketo将在Salesforce中创建重复的潜在客户，并将其分配给潜在客户队列。
   >
   >1. 如果您使用 **更改所有者** 联系人流程步骤，Marketo会在Salesforce中创建重复的潜在客户。 要避免这种情况，请在“SFDC类型”字段上使用过滤器，该过滤器将操作限制为仅潜在客户。

   >[!NOTE]
   >
   >如果您的Salesforce帐户中尚未存在该记录，我们会将其同步到此处，然后将其分配给选定的用户。
