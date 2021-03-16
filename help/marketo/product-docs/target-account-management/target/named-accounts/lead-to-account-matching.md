---
unique-page-id: 11381156
description: 客户匹配 — Marketo Docs — 产品文档
title: 潜在客户到帐户匹配
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 帐户匹配{#lead-to-account-matching}

使用Marketo Lead到帐户匹配将右潜在客户匹配到右指定帐户。

>[!NOTE]
>
>**Lead-to-Account Matchingis是Marketo** 目标 Account Management的内置功能。它采用模糊逻辑，在接近实时的情况下自动匹配出正确的指定帐户。 这些指定帐户可以是CRM帐户或Marketo公司。

Marketo销售线索到帐户匹配遵循4个步骤流程：

**第1步 — 我** 们的匹配流程首先使用潜在客户记录中的关键信息，例如：

* 电子邮件域（例如acme.com）
* 从IP地址推断公司名
* 公司名称 — 这可以是CRM帐户名或潜在客户公司名称属性（例如，来自表单填写）

**第2步 — 我** 们根据各种潜在客户属性（例如，Acme Inc.和Acme Corp将自动标准化为Acme）标准化我们查找的公司名称。此步骤可确保我们在Marketo中具有指定帐户的单一表示形式，并可以查看单个指定帐户中的所有潜在客户。

**第3步 — 我** 们将分区匹配Lead到2个存储段：强比赛和弱比赛。

* 弱匹配的潜在客户显示在指定帐户上，然后可以手动解析这些帐户。

**第4步 — 我** 们给出了强匹配和弱匹配的公司。当根据某个建议的公司创建指定帐户时，我们会创建匹配规则，以自动将新潜在客户（例如，已填写表单的潜在客户）转发到正确的指定帐户。 这样，您就不必再担心匹配潜在客户，而更担心获得收入！

由于Marketo Lead-to-Account匹配是Marketo目标帐户管理的内置功能，因此匹配Lead到帐户的操作几乎是实时的（例如，当Lead填写Marketo表单时，我们将Lead与正确的指定帐户关联）。 此事件可用于触发警报并通知帐户所有者新潜在客户从其指定帐户传入。

>[!NOTE]
>
>如果您在Salesforce中使用LeanData进行“潜在客户到帐户”匹配，则Marketo的集成会将这些匹配同步到您的Marketo实例。 要启用该功能，请联系[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)。

>[!MORELIKETHIS]
>
>[Discover帐户](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
