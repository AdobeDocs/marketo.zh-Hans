---
unique-page-id: 1147021
description: 更改所有者 — Marketo文档 — 产品文档
title: 更改所有者
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 更改所有者 {#change-owner}

如果您现有的人员已分配给所有者，则可以使用此流程步骤将它们重新分配给其他所有者。

![](assets/change-owner-1.png)

1. 只需选择所有者或您要更改为的潜在客户队列即可开始！

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >Salesforce不允许将联系人分配给潜在客户队列。 对于SFDC联系人记录：
   >
   >* 当联系人同步到Salesforce时，Marketo将仅创建重复的潜在客户&#x200B;**1}。**&#x200B;换句话说，如果您将&#x200B;**[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;流程步骤与`AssignTo=<a lead queue>`一起使用，则Marketo将在Salesforce中创建重复的潜在客户并将其分配给潜在客户队列。
   >
   >* 如果您对联系人使用&#x200B;**[!UICONTROL 更改所有者]**&#x200B;流程步骤，Marketo会在Salesforce中创建重复的潜在客户。 要避免这种情况，请在“SFDC类型”字段上使用过滤器，该过滤器将操作限制为仅潜在客户。

   >[!NOTE]
   >
   >如果您的Salesforce帐户中尚未存在该记录，我们会将其同步到此处，然后将其分配给选定的用户。
