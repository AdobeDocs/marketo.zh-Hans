---
unique-page-id: 1147344
description: 系统令牌术语表 — Marketo文档 — 产品文档
title: 系统令牌术语表
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
source-git-commit: 93032a016a67fe0edf7a8093633d6b06ec25c18d
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# 系统令牌术语表 {#system-tokens-glossary}

除了人员令牌之外，您还可以使用一些非常酷的系统令牌。 他们来了。

>[!NOTE]
>
>您的帐户时区设置会影响运行日期和时间令牌的时间。

## system.date {#system-date}

的 `{{system.date}}` 令牌在运行时将呈现当前日期，如下所示： **2013年8月08日**

**适用于：**

* [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;}流步骤
* [有趣的时刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;}流步骤
* [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;}流步骤
* 电子邮件或模板的正文

## system.time {#system-time}

的 `{{system.time}}` 令牌在运行时将呈现当前时间，如下所示： **04:34 PM(GMT -0700)**

**适用于：**

* [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;}流步骤
* [有趣的时刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;}流步骤
* [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;}流步骤
* 电子邮件或模板的正文

## system.dateTime {#system-datetime}

的 `{{system.dateTime}}` 令牌在运行时将呈现当前日期和时间，如下所示： **2013-08-08 16:36:13**

**适用于：**

* [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target=&quot;_blank&quot;}流步骤
* [有趣的时刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target=&quot;_blank&quot;}流步骤
* [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target=&quot;_blank&quot;}流步骤
* 电子邮件或模板的正文

## system.forwardToFriendLink {#system-forwardtofriendlink}

的 `{{system.forwardToFriendLink}}` 令牌允许您控制 [电子邮件中的“转发到朋友链接”](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target=&quot;_blank&quot;}。

**适用于：**

* [在电子邮件中将系统令牌添加为链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;}或模板

## system.unsubscribeLink {#system-unsubscribelink}

的 `{{system.unsubscribeLink}}` 令牌允许您控制取消订阅链接在电子邮件中的放置位置。

**适用于：**

* [在电子邮件中将系统令牌添加为链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;}或模板

## system.viewAsWebpageLink {#system-viewaswebpagelink}

的 `{{system.viewAsWebpageLink}}` 令牌允许您控制在电子邮件中显示“查看为网页”链接的位置。

**适用于：**

* [在电子邮件中将系统令牌添加为链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;}或模板
