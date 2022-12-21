---
unique-page-id: 14352592
description: 如何插入动态字段 — Marketo文档 — 产品文档
title: 如何插入动态字段
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 如何插入动态字段 {#how-to-insert-dynamic-fields}

我们允许您使用诸如之类的预定义属性来个性化电子邮件模板 `{{first_name}}` 或 `{{company}}`. 这些字段允许您通过电子邮件发送多个联系人并自动填写这些字段，而无需为每个联系人单独键入这些字段。

>[!TIP]
>
>“first_name”和“company”字段是唯一同时考虑Sales Connect和Salesforce的字段。 这意味着如果 [Web应用程序](https://toutapp.com/login)，我们会在Salesforce中查看我们是否可以找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，我们使用该记录中的信息来填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在 **模板和营销活动**，找到要编辑的模板并单击 **编辑模板**.

1. 单击 **输出动态字段**.

   >[!NOTE]
   >
   >向Sales Connect中存在的联系人发送电子邮件时，您可以使用基本的动态字段。 这些将直接从联系人处获取。

如果您向Salesforce中存在的联系人发送电子邮件，则可以利用Salesforce动态字段。 这些都以“sfdc”开头。 只要您与Salesforce建立连接，这些字段就会直接致电Salesforce中的潜在客户/联系人，以填充模板中的信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，请务必确保格式正确。
