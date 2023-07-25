---
unique-page-id: 1147344
description: 系统令牌术语表 — Marketo文档 — 产品文档
title: 系统令牌术语表
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 系统令牌术语表 {#system-tokens-glossary}

除了个人令牌之外，您还可以使用一些非常酷的系统令牌。 他们来了。

>[!NOTE]
>
>您的帐户时区设置会影响日期和时间令牌的运行时间。

## system.date {#system-date}

此 `{{system.date}}` 令牌将在运行时呈现当前日期，如下所示： **2013年8月8日**

**在以下位置工作：**

* [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} 流程步骤
* [有趣的时刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} 流程步骤
* [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程步骤
* 电子邮件或模板的正文

## system.time {#system-time}

此 `{{system.time}}` 令牌将在运行时呈现当前时间，如下所示： **下午04:34 （格林威治标准时间–0700）**

**在以下位置工作：**

* [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} 流程步骤
* [有趣的时刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} 流程步骤
* [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程步骤
* 电子邮件或模板的正文

## system.dateTime {#system-datetime}

此 `{{system.dateTime}}` 令牌将在运行时呈现当前日期和时间，如下所示： **2013-08-08 16:36:13**

**在以下位置工作：**

* [更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} 流程步骤
* [有趣的时刻](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} 流程步骤
* [创建任务](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} 流程步骤
* 电子邮件或模板的正文

## system.forwardToFriendLink {#system-forwardtofriendlink}

此 `{{system.forwardToFriendLink}}` 令牌允许您控制 [电子邮件中的“转发至朋友链接”](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**在以下位置工作：**

* [添加系统令牌作为电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} 或模板

## system.unsubscribeLink {#system-unsubscribelink}

此 `{{system.unsubscribeLink}}` 令牌允许您控制取消订阅链接在电子邮件中的放置。

**在以下位置工作：**

* [添加系统令牌作为电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} 或模板

## system.viewAsWebpageLink {#system-viewaswebpagelink}

此 `{{system.viewAsWebpageLink}}` 通过令牌，可控制电子邮件中以Web页形式查看链接的放置。

**适用于：**

* [添加系统令牌作为电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} 或模板
