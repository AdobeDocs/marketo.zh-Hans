---
description: 为什么我的动态字段没有填写？ - Marketo文档 — 产品文档
title: 为什么我的动态字段没有填写？
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 为什么我的动态字段没有填写？ {#why-arent-my-dynamic-fields-filling-out}

仅当使用模板时，动态字段才有效。 您编写的单次性电子邮件不会填写这些内容。

## 检查内容 {#what-to-check}

Sales Insight Actions中有三种类型的动态字段： Basic 、 Custom和Salesforce。 “基本”和“自定义”选项均可以从 [Web应用程序](https://toutapp.com/login){target="_blank"}. If the information does not exist in the web application, the fields will be blank. Salesforce fields pull information from [Salesforce.com](https://salesforce.com){target="_blank"}.

**Salesforce字段疑难解答**

Salesforce字段：例如 `{{sfdc_account_name}}`

* 确保正确地将其与Sales Insight Actions联系起来。 转到 [设置](https://toutapp.com/login{target="_blank"} 页面并单击 **管理** ，位于您的CRM旁边。

**基本和自定义字段故障诊断**

Marketo销售分析操作基本字段：例如， `{{company}}`

Marketo销售分析操作自定义字段：例如， `{{custom_field_favorite_movie}}`

* 需要为联系人保存的相应字段位于 [人员页面](https://toutapp.com/next#relationships){target="_blank"} 供动态域参考。 例如，如果您向Mary发送电子邮件并使用 `{{company}}` 字段，但她的联系记录未列出公司，我们无法填写。

## 为什么我的电子邮件没有填充所有动态字段就发送了？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我们无法填充电子邮件中的所有动态字段，则“销售分析操作”将阻止发送您的电子邮件。 **但是**&#x200B;有一些例外情况。 某些字段将发送空白，或者，如果我们可以找到某个值，则会自动填充该值。 下面列出了这些字段以及在无法填充该字段时它们将如何响应。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` =“您的公司”

`{{friendly_company}}` =“您的公司”

>[!NOTE]
>
>此 `{{first_name}}` 字段将同时在Sales Insight Actions和Salesforce中查找尝试提取信息的操作。 此列表中的所有其他字段仅查找销售分析操作以填充该字段。
