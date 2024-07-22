---
unique-page-id: 2953465
description: SFDC同步 — 在Salesforce中将潜在客户转化为联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 在Salesforce中将潜在客户转换为联系人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# SFDC同步：在Salesforce中将潜在客户转换为联系人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想像一下Salesforce中的三种不同场景：(不使用Marketo Engage中的[转化人员流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"})

1. 正在将潜在客户转换为&#x200B;**新联系人和新帐户**
1. 正在将潜在客户转换为&#x200B;**现有帐户**&#x200B;中的&#x200B;**新联系人**

1. 正在将Lead转换为&#x200B;**现有帐户**&#x200B;中的&#x200B;**现有联系人** （此操作与[合并](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"}的工作方式相同）

在所有三种情况下，您最终都将在Salesforce中找到&#x200B;**1位联系人且没有销售线索，在Marketo中找到1位联系人且没有联系人。**

在Marketo中，记录现在将具有SFDC类型= Contact。

>[!TIP]
>
>在Salesforce中转换时，请确保您的[潜在客户自定义字段映射正确](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}。 您不希望丢失任何数据。

您可以使用“Lead is Converted”和“Lead was Converted”来触发和筛选。
