---
unique-page-id: 1147344
description: 系统令牌词汇表- Marketo Docs —— 产品文档
title: 系统令牌词汇表
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 系统令牌词汇表 {#system-tokens-glossary}

除了个人令牌之外，您还可以使用一些非常酷的系统令牌。 他们来了。

>[!NOTE]
>
>帐户时区设置会影响运行日期和时间令牌的时间。

## system.date {#system-date}

令牌 `{{system.date}}` 将在运行时呈现当前日期，如下所示： **2013年8月8日**

**适用于：**

* [更改数据值流](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 步骤
* [有趣的矩](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) 流步骤
* [创建任务](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流步骤
* 电子邮件或模板的正文

## system.time {#system-time}

令牌 `{{system.time}}` 将在运行时呈现当前时间，如下所示： **下午04:34(GMT -0700)**

**适用于：**

* [更改数据值流](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 步骤
* [有趣的矩](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) 流步骤
* [创建任务](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流步骤
* 电子邮件或模板的正文

## system.dateTime {#system-datetime}

令牌 `{{system.dateTime}}` 将在运行时呈现当前日期和时间，如下所示： **2013-08-08 16:36:13**

**适用于：**

* [更改数据值流](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) 步骤
* [有趣的矩](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) 流步骤
* [创建任务](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) 流步骤
* 电子邮件或模板的正文

## system.forwardToFriendLink {#system-forwardtofriendlink}

此 `{{system.forwardToFriendLink}}` 令牌允许您控制“转发到朋 [友链接”在电子邮件中的位置](../../../../product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md)。

**适用于：**

* [将系统令牌添加为电子邮件或模板中的链](add-a-system-token-as-a-link-in-an-email.md) 接

## system.unsubscribeLink {#system-unsubscribelink}

令 `{{system.unsubscribLink}}` 牌允许您控制取消订阅链接在电子邮件中的位置。

**适用于：**

* [将系统令牌添加为电子邮件或模板中的链](add-a-system-token-as-a-link-in-an-email.md) 接

## system.viewAsWebpageLink {#system-viewaswebpagelink}

令牌 `{{system.viewAsWebpageLink}}` 允许您控制视图作为网页链接在电子邮件中的位置。

**适用于：**

* [将系统令牌添加为电子邮件或模板中的链](add-a-system-token-as-a-link-in-an-email.md) 接
