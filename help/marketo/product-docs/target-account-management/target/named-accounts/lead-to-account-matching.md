---
unique-page-id: 11381156
description: 潜在客户帐户匹配 — Marketo文档 — 产品文档
title: 商机帐户匹配
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 商机帐户匹配 {#lead-to-account-matching}

使用Marketo销售线索与帐户匹配将右销售线索与右指定帐户进行匹配。

>[!NOTE]
>
>**商机帐户匹配** 是Marketo Target帐户管理的内置功能。 它使用模糊逻辑来近乎实时地自动匹配指向正确指定帐户的潜在客户。 这些指定帐户可以是CRM帐户或Marketo公司。

## 概述 {#overview}

Marketo商机帐户匹配遵循4步流程：

**步骤1 -** 我们的配对过程从使用潜在客户记录上的关键信息开始，例如：

* 电子邮件域(例如，acme.com)
* 从IP地址推断出的公司名称
* 公司名称 — 这可以是CRM帐户名称或潜在客户公司名称属性（例如，来自表单填写）

**步骤2 -** 我们根据各种潜在客户属性对找到的公司名称进行标准化（例如，Acme Inc.和Acme Corp会自动标准化为Acme）。 此步骤可确保在Marketo中拥有指定帐户的单个表示形式，并且可以在单个指定帐户中查看所有潜在客户。

**步骤3 -** 我们将匹配的潜在客户划分为2个分段：强匹配和弱匹配。

* 弱匹配潜在客户出现在指定帐户上，然后可以手动解决。

**步骤4 -** 我们提供了一份拟议中的强弱匹配公司的名单。 当基于其中一家提议的公司创建指定帐户时，我们会创建匹配规则以自动将新的潜在客户（例如，填写表单的潜在客户）关联到正确的指定帐户。 这样，您就不必担心配对商机，而只需更多地担心如何获得收入！

由于Marketo销售线索与帐户配对是Marketo Target帐户管理的一项内置功能，因此对销售线索进行帐户配对几乎实时进行(例如，当销售线索填写Marketo表单时，我们会将所述的销售线索与正确的指定帐户相关联)。 此事件可用于触发警报，并向帐户所有者通知从其指定帐户传入的新潜在客户。

>[!NOTE]
>
>如果您使用Salesforce中的LeanData进行商机帐户匹配，则Marketo具有集成，该集成会将匹配项同步到您的Marketo实例。 要启用该功能，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 了解如何设置以下精益数据。

## 将精益数据用于销售线索与帐户匹配 {#using-leandata-for-lead-to-account-matching}

晚于 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 已为您的帐户启用LeanData，请按照以下步骤进行设置。

1. 在Salesforce中，单击 **设置主页** 左侧导航栏中。

1. 仍然在左侧导航栏中的“管理”下，单击 **用户** 则 **配置文件**.

1. 找到并选择 **Marketo同步** 个人资料。

1. 向下滚动到“字段级别安全性”部分，找到Lead对象。 选择 **视图**.

1. 对于字段名称“Reporting Matched Account”，确保 **读取权限** 列处于选中状态。

1. 在Marketo中，转到 **管理员** 部分。

   ![](assets/lead-to-account-matching-1.png)

1. 选择 **字段管理**.

   ![](assets/lead-to-account-matching-2.png)

1. 通过搜索“Reporting Matched Account”（报表匹配的帐户），确认字段存在。

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[发现帐户](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
