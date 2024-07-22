---
unique-page-id: 14352602
description: 我的动态字段未填写 — Marketo文档 — 产品文档
title: 我的动态字段未填写
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 我的动态字段未填写 {#my-dynamic-fields-arent-filling-out}

仅当使用模板时，动态字段才有效。 您编写的单次性电子邮件不会填写这些内容。

## 检查内容 {#what-to-check}

Sales Connect中有三种类型的动态字段： Basic 、 Custom和Salesforce。 “基本”和“自定义”都会从[Web应用程序](https://toutapp.com/login)中提取信息。 如果Web应用程序中不存在该信息，则字段将为空白。 Salesforce字段从[Salesforce.com](https://salesforce.com)提取信息。

**Salesforce字段疑难解答**

Salesforce字段：例如`{{sfdc_account_name}}`

* 确保正确地将其与Sales Connect连接起来。 转到[设置](https://toutapp.com/login)页面，然后单击CRM旁边的&#x200B;**管理**。

**基本和自定义字段疑难解答**

Tout基本字段：如`{{company}}`

Tout自定义字段：例如`{{custom_field_favorite_movie}}`

* 需要在[人员页面](https://toutapp.com/next#relationships)中为您的联系人保存对应的字段，以便我们的动态字段引用。 例如，如果您向Mary发送电子邮件并使用`{{company}}`字段，但她的联系记录未列出公司，则我们无法填写此信息。

## 为什么我的电子邮件没有填充所有动态字段就发送了？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我们无法在电子邮件中填充您的所有动态字段，则Sales Connect将停止发送您的电子邮件。 **但是**，此规则有一些例外。 某些字段将发送空白，或者，如果我们可以找到某个值，则会自动填充该值。 下面列出了这些字段以及在无法填充该字段时它们将如何响应。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>`{{first_name}}`字段将在Sales Connect和Salesforce中查找以尝试提取信息。 此列表中的所有其他字段仅在Sales Connect中查找以填充该字段。
