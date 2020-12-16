---
unique-page-id: 2953465
description: SFDC同步——在Salesforce中将潜在客户转换为联系人- Marketo文档——产品文档
title: SFDC同步——在Salesforce中将潜在客户转换为联系人
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# SFDC同步：在Salesforce中将潜在客户转换为联系人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想象Salesforce中的三种不同情况：(不使用Marketo [中的“转换人员流](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) ”步骤)

1. 将潜在客户转换为 **新联系人和新帐户**
1. 将潜在客户转换为现 **有帐户中** 的新 **联系人**

1. 将潜在客户转 **换为现有****帐户中的现有联系人** (这与合并 [工作相同](sfdc-sync-merging-a-lead-contact-person.md))

在这三种情况下，您最终在Salesforce **中都会遇到1个联系人，没有潜在客户，在Marketo中也会遇到1个联系人，没有任何人。**

在Marketo中，记录现在将具有SFDC类型=联系人。

>[!TIP]
>
>在Salesforce中进行转换时，请确保您的潜 [在客户自定义字段映射良好](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 您不希望丢失任何数据。

您可以使用以下方式触发和筛选：“潜在客户已转换”和“潜在客户已转换”。