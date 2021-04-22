---
unique-page-id: 2953465
description: SFDC同步 — 在Salesforce中将潜在客户转换为联系人 — Marketo文档 — 产品文档
title: SFDC同步 — 在Salesforce中将潜在客户转换为联系人
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC同步：在Salesforce中将潜在客户转换为联系人{#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

想象一下Salesforce中的三种不同情形：(未在Marketo中使用“转换人员流”步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md))[

1. 将潜在客户转换为&#x200B;**新联系人和新帐户**
1. 将Lead转换为&#x200B;**现有帐户**&#x200B;中的&#x200B;**新联系人**

1. 将Lead转换为&#x200B;**现有帐户**&#x200B;中的&#x200B;**现有联系人**（这与[合并](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md)工作相同）

在这三种情况下，您最终在Salesforce中都会遇到&#x200B;**1个联系人，没有潜在客户，在Marketo中则会遇到1个联系人。**

在Marketo中，记录现在将具有SFDC类型=联系人。

>[!TIP]
>
>在Salesforce中转换时，请确保[潜在客户自定义字段映射良好](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 您不希望丢失任何数据。

您可以使用以下方式触发和筛选：“潜在客户已转换”和“潜在客户已转换”。
