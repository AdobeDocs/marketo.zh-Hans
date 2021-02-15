---
unique-page-id: 14352602
description: 我的动态字段未填写 — Marketo Docs — 产品文档
title: 我的动态字段未填写
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# 我的动态字段未填写{#my-dynamic-fields-arent-filling-out}

只有在您使用模板时，动态字段才会生效。 您所写的个别一次性电子邮件无法填写这些内容。

## 检查{#what-to-check}的内容

Sales Connect中有三种类型的动态字段：基本、自定义和Salesforce。 “基本”和“自定义”均从[Web应用程序](https://toutapp.com/login)中提取信息。 如果Web应用程序中不存在该信息，则这些字段将为空。 Salesforce字段从[Salesforce.com](https://salesforce.com)提取信息。

**疑难解答Salesforce字段**

Salesforce字段：例如`{{sfdc_account_name}}`

* 确保它与Sales Connect正确连接。 转到[设置](https://toutapp.com/login)页面，然后单击CRM旁的&#x200B;**管理**。

**基本和自定义字段疑难解答**

输出基本字段：例如`{{company}}`

输出自定义字段：例如`{{custom_field_favorite_movie}}`

* 需要在[人物页面](https://toutapp.com/next#relationships)中为您的联系人保存相应的字段，以便我们的动态字段引用。 例如，如果您向Mary发送电子邮件并使用`{{company}}`字段，但她的联系记录不列表公司，我们将无法填写。

## 为什么在不填充所有动态字段的情况下发送电子邮件？{#why-did-my-email-send-without-populating-all-dynamic-fields}

如果我们无法在电子邮件中填充您的所有动态字段，Sales Connect将阻止您的电子邮件发送。 **但是**，此规则有一些例外。某些字段将发出空白，或者自动填充一个值（如果我们可以找到）。 下面列出了这些字段以及如果它们无法填充该字段将如何响应。

`{{first_name}}` =空

`{{last_name}}` =BLANK

`{{title}}` =空

`{{company}}` = &quot;您的公司&quot;

`{{friendly_company}}` = &quot;您的公司&quot;

>[!NOTE]
>
>`{{first_name}}`字段将在Sales Connect和Salesforce中查找以尝试提取信息。 此列表中的所有其他字段仅在Sales Connect中查找以填充该字段。
