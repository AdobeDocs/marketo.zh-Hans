---
unique-page-id: 14352592
description: 如何插入动态字段 — Marketo Docs — 产品文档
title: 如何插入动态字段
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 如何插入动态字段{#how-to-insert-dynamic-fields}

我们允许您使用预定义的属性（如`{{first_name}}`或`{{company}}`）个性化您的电子邮件模板。 这些字段允许您通过电子邮件发送多个联系人并自动填写这些字段，而不必为每个联系人单独键入这些字段。

>[!TIP]
>
>“first_name”和“公司”字段是将同时查看Sales Connect和Salesforce的唯一字段。 这意味着，如果[Web应用程序](https://toutapp.com/login)中不存在联系人，则我们会在Salesforce中查看我们是否能找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，我们使用该记录中的信息填充该字段。

## 将动态字段插入模板{#insert-a-dynamic-field-into-a-template}

1. 在&#x200B;**模板和活动**&#x200B;中，找到要编辑的模板，然后单击&#x200B;**编辑模板**。

1. 单击&#x200B;**输出动态字段**。

   >[!NOTE]
   >
   >向Sales Connect中存在的联系人发送电子邮件时，可以使用基本的动态字段。 这些会直接从联络人那里拉出来。

如果您正在向Salesforce中存在的联系人发送电子邮件，则可以利用Salesforce动态字段。 这些都以“sfdc”开头。 只要您与Salesforce有连接，这些字段将直接调用至Salesforce中的潜在客户/联系人，以在模板中填充信息。

## 在主题行{#insert-dynamic-fields-in-a-subject-line}中插入动态字段

只需手动将它们复制并粘贴到电子邮件的主题字段中，并确保格式正确。
