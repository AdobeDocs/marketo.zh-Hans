---
unique-page-id: 14352602
description: 我的动态字段未填写 — Marketo文档 — 产品文档
title: 我的动态字段没有填满
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# 我的动态字段没有填满 {#my-dynamic-fields-arent-filling-out}

仅当您使用模板时，动态字段才会起作用。 你写的个别一次性电子邮件不会填满这些内容。

## 要检查的内容 {#what-to-check}

Sales Connect中有三种类型的动态字段：基本、自定义和Salesforce。 基本和自定义功能均可从 [Web应用程序](https://toutapp.com/login). 如果Web应用程序中不存在该信息，则字段将为空。 Salesforce字段从中提取信息 [Salesforce.com](https://salesforce.com).

**Salesforce字段疑难解答**

Salesforce字段：例如 `{{sfdc_account_name}}`

* 确保它与Sales Connect正确挂接。 转到 [设置](https://toutapp.com/login) 页面，单击 **管理** 的CRM。

**基本和自定义字段故障诊断**

输出基本字段：例如 `{{company}}`

输出自定义字段：例如 `{{custom_field_favorite_movie}}`

* 需要为中的联系人保存相应的字段 [“人员”页面](https://toutapp.com/next#relationships) 供我们的动态字段参考。 例如，如果您向Mary发送电子邮件，并使用 `{{company}}` 但她的联系记录没有列出公司，我们无法填写。

## 为什么在不填充所有动态字段的情况下发送电子邮件？ {#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我们无法填充电子邮件中的所有动态字段，则Sales Connect将阻止发送电子邮件。 **但是**，则此规则有一些例外。 某些字段将发出空白，或者如果我们找到值，则自动填充值。 下面列出了这些字段以及它们在无法填充该字段时的反应方式。

`{{first_name}}` =空

`{{last_name}}` =BLANK

`{{title}}` =空

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>的 `{{first_name}}` 字段将在Sales Connect和Salesforce中查找以尝试提取信息。 此列表中的所有其他字段仅在Sales Connect中查看以填充该字段。
