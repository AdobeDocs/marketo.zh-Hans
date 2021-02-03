---
unique-page-id: 4719316
description: 使用人员帐户- Marketo Docs —— 产品文档
title: 使用人员帐户
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# 使用人员帐户{#using-person-accounts}

可以在Salesforce中设置人员帐户，以满足您组织的需求。 Marketo如何处理个人帐户。

>[!NOTE]
>
>默认的Salesforce帐户是业务帐户。 您的Salesforce管理员需要单独设置个人帐户。

## 什么是个人帐户？{#what-is-a-person-account}

人员帐户与Salesforce中的帐户对象非常相似。 但是，个人帐户可以访问帐户字段和联系人字段。

## 当个人帐户同步到Marketo时会发生什么情况？{#what-happens-when-a-person-account-is-synced-to-marketo}

人员帐户以公司和人员身份同步到Marketo。

>[!NOTE]
>
>人员帐户的自定义字段将复制到Marketo中的公司和人员。

## 如何区分业务帐户和个人帐户？{#how-do-i-differentiate-business-accounts-and-person-accounts}

在您的智能列表中使用&#x200B;**是人员帐户**&#x200B;过滤器，将人员帐户与标准业务帐户分开。

## 我的个人帐户信息在Marketo Sales Insight中显示在哪里？{#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

与个人帐户相关的活动显示在&#x200B;**帐户**&#x200B;面板中。

>[!NOTE]
>
>Marketo Sales Insight的&#x200B;**添加到Marketo活动**&#x200B;和&#x200B;**发送电子邮件**&#x200B;选项当前不适用于个人帐户。

## 如何将机会关联到个人帐户？{#how-do-i-associate-opportunities-to-a-person-account}

Marketo取决于业务机会联系人角色，以确定要将业务机会关联到的人员。 您需要为每个人员帐户添加机会联系人角色，以便将该机会连接到Marketo中的适当人员。 我们建议您设置一个工作流以自动添加业务机会联系人角色。

## 我应将哪个电子邮件字段用于个人帐户？{#which-email-field-should-i-use-for-person-accounts}

个人帐户有两个电子邮件字段。 使用表单中的&#x200B;**电子邮件地址**&#x200B;字段（不是&#x200B;**人员电子邮件地址**）可确保Marketo的重复数据消除和其他电子邮件处理正常工作。
