---
unique-page-id: 14352592
description: 如何插入动态字段- Marketo Docs —— 产品文档
title: 如何插入动态字段
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# 如何插入动态字段 {#how-to-insert-dynamic-fields}

我们允许您使用预定义的属性（如或）来个性化您 `{{first_name}}` 的电子邮件 `{{company}}`模板。 这些字段允许您通过电子邮件发送多个联系人并自动填写这些字段，而不必为每个联系人单独键入这些字段。

>[!TIP]
>
>“first_name”和“公司”字段是 `only fields that will look to both Sales Connect and Salesforce.` “That”表示，如果Web应用程序中不存在联系人 [](http://toutapp.com/login)，我们会在Salesforce中查看我们是否能找到具有匹配电子邮件地址的联系人／潜在客户记录。 然后，我们使用该记录中的信息填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在“ **模板和活动**”中，找到要编辑的模板，然后单击“编 **辑模板”**。
1. 单击“ **输出动态字段**”。

   >[!NOTE]
   >
   >在向Sales Connect中存在的联系人发送电子邮件时，可以使用基本的动态字段。 这些会直接从联系人处拉出。

如果您正在向Salesforce中存在的联系人发送电子邮件，则可以利用Salesforce动态字段。 这些都以“sfdc”开头。 只要您与Salesforce有连接，这些字段将直接调用Salesforce中的潜在客户／联系人以在模板中填充信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，确保您具有正确的格式。
