---
unique-page-id: 2953465
description: SFDC同步 — 在Salesforce中将潜在客户转换为联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 在Salesforce中将潜在客户转换为联系人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce中将潜在客户转换为联系人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想象一下Salesforce中的三种不同情形：(不使用 [转换人员流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) 在Marketo)

1. 将潜在客户转换为 **新联系人和新帐户**
1. 将潜在客户转换为 **新联系人** 在 **现有帐户**

1. 将潜在客户转换为 **现有联系人** 在 **现有帐户** (这与 [合并](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

在这三种情况中 **在Salesforce中有1个联系人，没有潜在客户，在Marketo有1个联系人，没有人员。**

在Marketo中，记录现在将具有SFDC类型=联系人。

>[!TIP]
>
>在Salesforce中转换时，请确保 [潜在客户自定义字段映射良好](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). 您不希望丢失任何数据。

您可以使用以下方法触发和过滤：“潜在客户已转化”和“潜在客户已转化”。
