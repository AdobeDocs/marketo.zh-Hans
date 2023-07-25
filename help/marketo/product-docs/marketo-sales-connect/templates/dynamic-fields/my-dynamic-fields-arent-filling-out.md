---
unique-page-id: 14352602
description: 我的动态字段未填写 — Marketo文档 — 产品文档
title: 我的动态字段未填写
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# 我的动态字段未填写 {#my-dynamic-fields-arent-filling-out}

仅当使用模板时，动态字段才有效。 您编写的单独一次性电子邮件不会填写这些内容。

## 检查内容 {#what-to-check}

Sales Connect中有三种类型的动态字段： Basic 、 Custom和Salesforce。 Basic和Custom都希望从 [Web应用程序](https://toutapp.com/login). 如果Web应用程序中不存在该信息，则字段将为空。 Salesforce字段提取信息来源 [Salesforce.com](https://salesforce.com).

**Salesforce字段疑难解答**

Salesforce字段：例如 `{{sfdc_account_name}}`

* 确保正确连接到Sales Connect。 转到 [设置](https://toutapp.com/login) 页面并单击 **管理** ，位于您的CRM旁边。

**基本和自定义字段故障诊断**

介绍基本字段：例如 `{{company}}`

吹嘘自定义字段：例如 `{{custom_field_favorite_movie}}`

* 需要为您的联系人保存相应的字段 [人员页面](https://toutapp.com/next#relationships) 供动态域参考。 例如，如果您向Mary发送电子邮件，并使用 `{{company}}` 字段，但她的联系记录未列出公司，我们无法填写。

## 为什么我的电子邮件发送时没有填充所有动态字段？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我们无法填充电子邮件中的所有动态字段，Sales Connect将阻止发送您的电子邮件。 **但是**，但此规则有一些例外。 某些字段将发送空白内容，或者如果我们可以找到某个值，则自动填充该值。 以下列出了这些字段以及在无法填充该字段时它们将如何反应。

`{{first_name}}` =空白

`{{last_name}}` =BLANK

`{{title}}` =空白

`{{company}}` =“您的公司”

`{{friendly_company}}` =“您的公司”

>[!NOTE]
>
>此 `{{first_name}}` 字段将同时查看Sales Connect和Salesforce以尝试提取信息。 此列表中的所有其他字段仅在Sales Connect中查找以填充该字段。
