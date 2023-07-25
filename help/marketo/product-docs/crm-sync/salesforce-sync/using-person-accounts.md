---
unique-page-id: 4719316
description: 使用人员帐户 — Marketo文档 — 产品文档
title: 使用人员帐户
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用人员帐户 {#using-person-accounts}

可在Salesforce中设置人员帐户以满足贵组织的需要。 以下是Marketo处理个人帐户的方式。

>[!NOTE]
>
>默认的Salesforce帐户是业务帐户。 您的Salesforce管理员需要单独设置人员帐户。

## 什么是个人帐户？ {#what-is-a-person-account}

人员帐户与Salesforce中的帐户对象非常相似。 但是，人员帐户对帐户字段和联系人字段均具有访问权限。

## 将人员帐户同步到Marketo后会出现什么情况？ {#what-happens-when-a-person-account-is-synced-to-marketo}

人员帐户作为公司和人员同步到Marketo。

>[!NOTE]
>
>人员帐户的自定义字段将会复制到Marketo中的公司和人员。

## 如何区分业务帐户和个人帐户？ {#how-do-i-differentiate-business-accounts-and-person-accounts}

使用 **是人员帐户** 在智能列表中进行筛选，以将人员帐户与标准业务帐户分开。

## 我的个人帐户信息在Marketo Sales Insight中的什么位置显示？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

与人员帐户相关的活动显示在 **帐户** 面板。

>[!NOTE]
>
>Marketo Sales Insight的 **添加到Marketo Campaign** 和 **发送电子邮件** 选项当前不可用于人员帐户。

## 如何将机会与人员帐户关联？ {#how-do-i-associate-opportunities-to-a-person-account}

Marketo依赖于机会联系人角色来确定要将机会与哪个人员相关联。 您需要为每个人员帐户添加机会联系人角色，以将机会连接到Marketo中的适当人员。 我们建议您设置一个工作流以自动添加机会联系人角色。

## 个人帐户应使用哪个电子邮件字段？ {#which-email-field-should-i-use-for-person-accounts}

人员帐户有两个电子邮件字段。 使用 **电子邮件地址** 表单中的字段(而不是 **人员电子邮件地址**)，以确保Marketo的重复数据消除和其他电子邮件处理正常工作。
