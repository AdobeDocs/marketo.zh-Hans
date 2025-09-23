---
unique-page-id: 14352592
description: 如何插入动态字段 — Marketo文档 — 产品文档
title: 如何插入动态字段
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 4%

---

# 如何插入动态字段 {#how-to-insert-dynamic-fields}

我们允许您使用预定义属性（如`{{first_name}}`或`{{company}}`）个性化电子邮件模板。 这些字段允许您向多个联系人发送电子邮件，并自动完成这些字段，而无需为每个联系人单独键入它们。

>[!TIP]
>
>“first_name”和“company”字段是仅有的将同时查找[!DNL Sales Connect]和[!DNL Salesforce]的字段。 这意味着，如果[Web应用程序](https://toutapp.com/login)中不存在联系人，我们会查看[!DNL Salesforce]，以查看是否可以找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，使用该记录中的信息来填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在&#x200B;**[!UICONTROL Templates & Campaigns]**&#x200B;中，找到要编辑的模板并单击&#x200B;**[!UICONTROL Edit Template]**。

1. 单击 **[!UICONTROL Tout Dynamic Fields]**。

   >[!NOTE]
   >
   >通过电子邮件发送存在于[!DNL Sales Connect]中的联系人时，您可以使用基本动态字段。 这些将直接从联系人中提取。

如果您要通过电子邮件发送存在于[!DNL Salesforce]中的联系人，则可以利用[!DNL Salesforce]动态字段。 所有这些都以“sfdc”开头。 只要您连接到[!DNL Salesforce]，这些字段就会直接调用[!DNL Salesforce]中的潜在客户/联系人以填充模板中的信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，注意确保设置正确的格式。
