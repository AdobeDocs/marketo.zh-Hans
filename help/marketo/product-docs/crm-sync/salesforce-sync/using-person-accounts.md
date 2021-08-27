---
unique-page-id: 4719316
description: 使用人员帐户 — Marketo文档 — 产品文档
title: 使用人员帐户
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 使用人员帐户 {#using-person-accounts}

可以在Salesforce中设置人员帐户，以满足您组织的需求。 这是Marketo对待个人账户的方式。

>[!NOTE]
>
>默认的Salesforce帐户是业务帐户。 您的Salesforce管理员需要单独设置人员帐户。

## 什么是个人帐户？ {#what-is-a-person-account}

人员帐户与Salesforce中的帐户对象非常相似。 但是，个人帐户同时具有帐户字段和联系字段的访问权限。

## 当人员帐户同步到Marketo时，会出现什么情况？ {#what-happens-when-a-person-account-is-synced-to-marketo}

人员帐户以公司和人员身份同步到Marketo。

>[!NOTE]
>
>人员帐户的自定义字段会复制到Marketo中的公司和人员。

## 如何区分业务帐户和人员帐户？ {#how-do-i-differentiate-business-accounts-and-person-accounts}

在智能列表中使用&#x200B;**是人员帐户**&#x200B;过滤器，将人员帐户与标准业务帐户分开。

## 我的人员帐户信息在Marketo Sales Insight中显示在哪里？ {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

与人员帐户相关的活动显示在&#x200B;**帐户**&#x200B;面板中。

>[!NOTE]
>
>Marketo Sales Insight的&#x200B;**添加到Marketo Campaign**&#x200B;和&#x200B;**发送电子邮件**&#x200B;选项当前不适用于人员帐户。

## 如何将机会与个人帐户关联？ {#how-do-i-associate-opportunities-to-a-person-account}

Marketo取决于机会联系角色来确定要将机会关联到的人员。 您需要为每个人员帐户添加机会联系角色，以将该机会与Marketo中的相应人员连接起来。 我们建议您设置一个工作流以自动添加机会联系角色。

## 我应该将哪个电子邮件字段用于个人帐户？ {#which-email-field-should-i-use-for-person-accounts}

个人帐户有两个电子邮件字段。 使用表单中的&#x200B;**电子邮件地址**&#x200B;字段（而不是&#x200B;**人员电子邮件地址**），确保Marketo的重复数据删除和其他电子邮件处理正常工作。
