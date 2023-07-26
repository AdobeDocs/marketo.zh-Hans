---
unique-page-id: 2953465
description: SFDC同步 — 在Salesforce中将潜在客户转化为联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 在Salesforce中将潜在客户转换为联系人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce中将潜在客户转换为联系人 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想像一下Salesforce中的三种不同场景：(不使用 [转换人员流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) (在Marketo中)

1. 将潜在客户转化为 **新联系人和新帐户**
1. 将潜在客户转化为 **新建联系人** 在 **现有帐户**

1. 将潜在客户转换为 **现有联系人** 在 **现有帐户** (此工作方式与 [合并](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

在所有三个案例中 **Salesforce中存在1个联系人且没有潜在客户，Marketo中存在1个联系人且没有人员。**

在Marketo中，记录现在将具有SFDC类型= Contact。

>[!TIP]
>
>在Salesforce中转换时，请确保您的 [商机自定义字段映射良好](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). 您不希望丢失任何数据。

您可以使用“Lead is Converted”和“Lead was Converted”来触发和筛选。
