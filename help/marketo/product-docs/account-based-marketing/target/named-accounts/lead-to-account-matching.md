---
unique-page-id: 11381156
description: Lead to Account Matching - Marketo Docs - Product Documentation
title: 客户匹配潜在客户
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 导致帐户匹配{#lead-to-account-matching}

使用“营销人员潜在客户到帐户”匹配右侧潜在客户到右侧指定帐户。

>[!NOTE]
>
>**“客户到帐户”** Matchingis是基于Marketo帐户的营销的内置功能。它采用模糊逻辑，几乎实时地自动将潜在客户与正确的指定帐户匹配。 这些指定帐户可以是CRM帐户或Marketo公司。

Marketo Lead-to-Account Matching遵循4个步骤流程：

**第1步——我** 们的匹配流程首先使用潜在客户记录的关键信息，例如：

* 电子邮件域（例如acme.com）
* 从IP地址推断公司名
* 公司名称——这可以是CRM帐户名称或潜在客户公司名称属性（例如，来自表单填写）

**第2步-** 我们根据各种潜在客户属性（例如，Acme Inc.和Acme Corp自动标准化为Acme）标准化我们查找的公司名称。此步骤确保我们在Marketo中具有指定帐户的单一表示形式，并可以查看单个指定帐户中的所有潜在客户。

**第3步——我** 们将匹配的Lead分为2个存储段：强与弱。

* 弱匹配的潜在客户显示在指定的帐户上，然后可以手动解析这些帐户。

**第4步——我** 们给出了一个强弱匹配的公司列表。当根据某个建议的公司创建指定帐户时，我们会创建匹配规则，以自动将新潜在客户（例如，已填写表单的潜在客户）转发到正确的指定帐户。 这样，您就不必再为匹配潜在客户而担心更多地为获得收入！

由于“营销人员潜在客户到帐户”匹配是“基于营销人员帐户的营销”的内置功能，因此，匹配销售线索到帐户的操作几乎实时进行（例如，当潜在客户填写营销人员表单时，我们会将所述销售线索与正确的指定帐户关联）。 此事件可用于触发警报并通知帐户所有者新潜在客户从其指定帐户中传入。

>[!NOTE]
>
>如果您在Salesforce中使用LeanData进行潜在客户到帐户匹配，Marketo的集成会将这些匹配项同步到您的Marketo实例。 要启用该功能，请与[Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support)联系。

>[!MORELIKETHIS]
>
>[发现帐户](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md)
