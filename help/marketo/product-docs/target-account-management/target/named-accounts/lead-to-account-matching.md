---
unique-page-id: 11381156
description: 潜在客户帐户匹配 — Marketo文档 — 产品文档
title: 商机帐户匹配
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 商机帐户匹配 {#lead-to-account-matching}

使用Marketo销售线索与帐户匹配将右销售线索与右指定帐户匹配。

>[!NOTE]
>
>**商机帐户匹配**&#x200B;是Marketo [!UICONTROL Target Account Management]的内置功能。 它使用模糊逻辑近乎实时地自动匹配通向正确指定帐户的线索。 这些指定帐户可以是CRM帐户或Marketo公司。

## 概述 {#overview}

Marketo商机帐户匹配遵循以下4个步骤流程：

**步骤1 -**&#x200B;我们的配对过程首先使用潜在客户记录上的关键信息，例如：

* 电子邮件域(例如，acme.com)
* 从IP地址推断的公司名称
* 公司名称 — 这可以是CRM帐户名称或潜在客户公司名称属性（例如，来自表单填写）

**步骤2 -**&#x200B;我们根据各种潜在客户属性将找到的公司名称标准化（例如，Acme Inc.和Acme Corp自动标准化为Acme）。 此步骤确保我们在Marketo中有该指定帐户的单个表示形式，并且能够在单个指定帐户中查看所有潜在客户。

**步骤3 -**&#x200B;我们将匹配的潜在客户分区为2个分段：强匹配和弱匹配。

* 弱匹配潜在客户出现在指定帐户上，然后可以手动解析。

**步骤4 -**&#x200B;我们提供一个建议的公司列表，这些公司具有强匹配和弱匹配。 当根据其中一家提议的公司创建指定帐户时，我们会创建匹配规则以自动将新的潜在客户（例如，填写表单的潜在客户）关联到正确的指定帐户。 这样，您就可以更少地担心匹配潜在客户，而更担心获得收入！

由于Marketo商机与帐户匹配是Marketo [!UICONTROL Target Account Management]的一项内置功能，因此对商机与帐户的匹配几乎实时发生(例如，当商机填写Marketo表单时，我们会将该商机与正确的指定帐户相关联)。 此事件可用于触发警报，并向帐户所有者通知从其指定帐户传入的新潜在客户。

>[!NOTE]
>
>如果您使用Salesforce中的LeanData进行商机帐户匹配，Marketo将具有集成，该集成会将匹配项同步到您的Marketo实例。 要启用该功能，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)了解以下如何设置LeanData。

## 将精益数据用于销售线索与帐户匹配 {#using-leandata-for-lead-to-account-matching}

在[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)为您的帐户启用LeanData后，请按照以下步骤进行设置。

1. 在Salesforce中，单击左侧导航栏中的&#x200B;**[!UICONTROL Setup Home]**。

1. 仍然在左侧导航中的“管理”下，单击&#x200B;**[!UICONTROL Users]**，然后单击&#x200B;**[!UICONTROL Profiles]**。

1. 找到并选择&#x200B;**Marketo Sync**&#x200B;配置文件。

1. 向下滚动到“字段级安全性”部分，并找到Lead对象。 选择 **[!UICONTROL View]**。

1. 对于字段名称“报告匹配的帐户”，确保选中&#x200B;**[!UICONTROL Read Access]**&#x200B;列中的复选框。

1. 在Marketo中，转到&#x200B;**[!UICONTROL Admin]**&#x200B;部分。

   ![](assets/lead-to-account-matching-1.png)

1. 选择 **[!UICONTROL Field Management]**。

   ![](assets/lead-to-account-matching-2.png)

1. 通过搜索&quot;[!UICONTROL Reporting Matched Account]&quot;确认字段存在。

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[发现帐户](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
