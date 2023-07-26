---
unique-page-id: 11381156
description: 潜在客户帐户匹配 — Marketo文档 — 产品文档
title: 商机帐户匹配
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# 商机帐户匹配 {#lead-to-account-matching}

使用Marketo销售线索与帐户匹配将右销售线索与右指定帐户匹配。

>[!NOTE]
>
>**商机帐户匹配** 是Marketo Target帐户管理的内置功能。 它使用模糊逻辑近乎实时地自动匹配通向正确指定帐户的线索。 这些指定帐户可以是CRM帐户或Marketo公司。

## 概述 {#overview}

Marketo商机帐户匹配遵循以下4个步骤流程：

**步骤1 -** 我们的配对过程首先使用潜在客户记录上的关键信息，例如：

* 电子邮件域(例如，acme.com)
* 从IP地址推断的公司名称
* 公司名称 — 这可以是CRM帐户名称或潜在客户公司名称属性（例如，来自表单填写）

**第2步 —** 我们根据各种潜在客户属性（例如， Acme Inc.和Acme Corp自动标准化为Acme ）将找到的公司名称标准化。 此步骤确保我们在Marketo中有该指定帐户的单个表示形式，并且能够在单个指定帐户中查看所有潜在客户。

**步骤3 -** 我们将匹配的潜在客户划分为2个分段：强匹配和弱匹配。

* 弱匹配潜在客户出现在指定帐户上，然后可以手动解析。

**步骤4 -** 我们提供了一份拟议中的强弱匹配公司的名单。 当根据其中一家提议的公司创建指定帐户时，我们会创建匹配规则以自动将新的潜在客户（例如，填写表单的潜在客户）关联到正确的指定帐户。 这样，您就可以更少地担心匹配潜在客户，而更担心获得收入！

由于Marketo商机与帐户匹配是Marketo Target帐户管理的内置功能，因此匹配商机会近乎实时地发生帐户(例如，当商机填写Marketo表单时，我们会将该商机与正确的指定帐户关联)。 此事件可用于触发警报，并向帐户所有者通知从其指定帐户传入的新潜在客户。

>[!NOTE]
>
>如果您使用Salesforce中的LeanData进行商机帐户匹配，Marketo将具有集成，该集成会将匹配项同步到您的Marketo实例。 要启用该功能，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 了解如何在下方设置LeanData。

## 将精益数据用于销售线索与帐户匹配 {#using-leandata-for-lead-to-account-matching}

之后 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 已为您的帐户启用LeanData，请按照以下步骤进行设置。

1. 在Salesforce中，单击 **设置主页** 在左侧导航栏中。

1. 仍然在左侧导航栏中的“管理”下，单击 **用户** 则 **配置文件**.

1. 找到并选择 **Marketo同步** 个人资料。

1. 向下滚动到“字段级安全性”部分，并找到Lead对象。 选择 **视图**.

1. 对于字段名称“Reporting Matched Account”，确保 **读取权限** 列处于选中状态。

1. 在Marketo中，转到 **管理员** 部分。

   ![](assets/lead-to-account-matching-1.png)

1. 选择 **字段管理**.

   ![](assets/lead-to-account-matching-2.png)

1. 通过搜索“Reporting Matched Account”（报表匹配帐户），确认字段存在。

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[发现帐户](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
