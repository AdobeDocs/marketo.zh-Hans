---
unique-page-id: 4719314
description: 默认Salesforce字段映射 — Marketo文档 — 产品文档
title: 默认Salesforce字段映射
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 2%

---

# 默认[!DNL Salesforce]字段映射 {#default-salesforce-field-mapping}

当您最初将Marketo Engage帐户与Salesforce同步时，Marketo会自动在内置的Salesforce和Marketo字段之间建立这些关联。 Marketo还将同步您的Leads、Accounts、Opportunities和Contacts上的自定义字段。

## 潜在客户字段 {#lead-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| [!UICONTROL Annual Revenue] | [!UICONTROL Annual Revenue] |
| [!UICONTROL City] | [!UICONTROL City] |
| [!UICONTROL Company] | [!UICONTROL Company Name] |
| [!UICONTROL Converted Date] | [!UICONTROL SFDC Converted Date] |
| [!UICONTROL Country] | [!UICONTROL Country] |
| [!UICONTROL Created Date] | [!UICONTROL SFDC Created Date] |
| [!UICONTROL Description] | [!UICONTROL Person Notes] |
| [!UICONTROL Email] | [!UICONTROL Email Address] |
| [!UICONTROL Fax] | [!UICONTROL Fax Number] |
| [!UICONTROL First Name] | [!UICONTROL First Name] |
| [!UICONTROL Email Opt Out] | [!UICONTROL Unsubscribed] |
| [!UICONTROL Industry] | [!UICONTROL Industry] |
| [!UICONTROL Converted] | [!UICONTROL SFDC Is Converted] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Last Name] | [!UICONTROL Last Name] |
| [!UICONTROL Lead Source] | [!UICONTROL Source] |
| [!UICONTROL Lead Score] | [!UICONTROL Score] |
| [!UICONTROL Mobile Phone] | [!UICONTROL Mobile Phone Number] |
| [!UICONTROL Employees] | [!UICONTROL Num Employees] |
| [!UICONTROL Phone] | [!UICONTROL Phone Number] |
| [!UICONTROL Zip/Postal Code] | [!UICONTROL Postal Code] |
| [!UICONTROL Rating] | [!UICONTROL Rating] |
| [!UICONTROL Salutation] | [!UICONTROL Salutation] |
| [!UICONTROL State/Province] | [!UICONTROL State] |
| [!UICONTROL Status] | [!UICONTROL Status] |
| [!UICONTROL Street] | [!UICONTROL Address] |
| [!UICONTROL Title] | [!UICONTROL Job Title] |
| [!UICONTROL Website] | [!UICONTROL Website] |

## 联系人字段 {#contact-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| [!UICONTROL Birthdate] | [!UICONTROL Date of Birth] |
| [!UICONTROL Created Date] | [!UICONTROL SFDC Created Date] |
| [!UICONTROL Contact Description] | [!UICONTROL Person Notes] |
| [!UICONTROL Email] | [!UICONTROL Email Address] |
| [!UICONTROL Business Fax] | [!UICONTROL Fax Number] |
| [!UICONTROL First Name] | [!UICONTROL First Name] |
| [!UICONTROL Email Opt Out] | [!UICONTROL Unsubscribed] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Last Name] | [!UICONTROL Last Name] |
| [!UICONTROL Lead Source] | [!UICONTROL Source] |
| [!UICONTROL Lead Score] | [!UICONTROL Score] |
| [!UICONTROL MailingCity] | [!UICONTROL City] |
| [!UICONTROL MailingCountry] | [!UICONTROL Country] |
| [!UICONTROL MailingPostalCode] | [!UICONTROL Postal Code] |
| [!UICONTROL MailingState] | [!UICONTROL State] |
| [!UICONTROL MailingStreet] | [!UICONTROL Address] |
| [!UICONTROL Mobile Phone] | [!UICONTROL Mobile Phone Number] |
| [!UICONTROL Business Phone] | [!UICONTROL Phone Number] |
| [!UICONTROL Salutation] | [!UICONTROL Salutation] |
| [!UICONTROL Title] | [!UICONTROL Job Title] |

## 帐户字段 {#account-fields}

| [!UICONTROL SFDC field] | [!UICONTROL Marketo field] |
|---|---|
| [!UICONTROL Annual Revenue] | [!UICONTROL Annual Revenue] |
| [!UICONTROL Billing City] | [!UICONTROL Billing City] |
| [!UICONTROL Billing Country] | [!UICONTROL Billing Country] |
| [!UICONTROL Billing Zip/Postal Code] | [!UICONTROL Billing Postal Code] |
| [!UICONTROL Billing State/Province] | [!UICONTROL Billing State] |
| [!UICONTROL Billing Street] | [!UICONTROL Billing Address] |
| [!UICONTROL Account Description] | [!UICONTROL Company Notes] |
| [!UICONTROL Industry] | [!UICONTROL Industry] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Account Name] | [!UICONTROL Company Name] |
| [!UICONTROL Employees] | [!UICONTROL Num Employees] |
| [!UICONTROL Account Phone] | [!UICONTROL Main Phone] |
| [!UICONTROL SIC Code] | [!UICONTROL SIC Code] |
| [!UICONTROL Account Site] | [!UICONTROL Site] |
| [!UICONTROL Account Type] | [!UICONTROL SFDC Type] |
| [!UICONTROL Website] | [!UICONTROL Website] |

## Marketo中与[!DNL Salesforce]相关的系统字段（只读） {#salesforce-related-system-fields-in-marketo-read-only}

这些字段是在Marketo中创建的，但无法由客户调整。

| 字段 | 描述 |
|---|---|
| SFDC Id | 由18个字符组成的[!DNL Salesforce] ID |
| SFDC 类型 | 潜在客户或联系人。 如果为空，则商机在Marketo中仅作为人员存在 |
| SFDC创建日期 | 在SFDC中创建的日期(可以不同于在Marketo中创建的日期) |
| SFDC已删除 | 此人以前在SFDC中，但现在已被删除，仅居住在Marketo中 |
