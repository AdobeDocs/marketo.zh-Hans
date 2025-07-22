---
description: 动态字段 — Marketo文档 — 产品文档
title: 动态字段
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# 动态字段 {#dynamic-fields}

我们允许您使用预定义属性（如`{{first_name}}`或`{{company}}`）个性化电子邮件模板。 这些字段允许您向多个联系人发送电子邮件，并自动完成这些字段，而无需为每个联系人单独键入它们。

>[!TIP]
>
>“first_name”和“company”字段是仅有的将同时查找[!DNL Sales Insight Actions]和[!DNL Salesforce]的字段。 这意味着，如果[Web应用程序](https://toutapp.com/login)中不存在联系人，我们会查看[!DNL Salesforce]，以查看是否可以找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，使用该记录中的信息来填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在&#x200B;**[!UICONTROL Templates & Campaigns]**&#x200B;中，找到要编辑的模板并单击&#x200B;**[!UICONTROL Edit Template]**。

1. 单击 **[!UICONTROL Insert Dynamic Field]**。

   >[!NOTE]
   >
   >通过电子邮件发送存在于[!DNL Sales Insight Actions]中的联系人时，您可以使用基本动态字段。 这些将直接从联系人中提取。

如果您要通过电子邮件发送存在于[!DNL Salesforce]中的联系人，则可以利用[!DNL Salesforce]动态字段。 所有这些都以“sfdc”开头。 只要您连接到[!DNL Salesforce]，这些字段就会直接调用[!DNL Salesforce]中的潜在客户/联系人以填充模板中的信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，注意确保设置正确的格式。

## 动态字段默认值 {#dynamic-field-default-values}

将动态字段添加到电子邮件模板时，您可以添加一个默认值，如果没有其他可用值，动态字段将解析为该默认值。

为此，请在动态字段标签后添加“|”，然后添加“default：”（两者均不带引号）。 然后，如果找不到其他值，请添加您希望字段解析为的值（用引号括起来）。

**示例：**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 动态字段术语表 {#dynamic-fields-glossary}

在[!DNL Sales Insight Actions]中创建模板时，我们始终建议使用&#x200B;**[!UICONTROL Insert Dynamic Field]**&#x200B;按钮集成动态字段。

此工具用于`auto-personalize your email`，并由`pulling information from the People page`为您节省大量时间。

| 动态字段 | 电子邮件中显示内容示例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | 如果您不想再收到我们的电子邮件，请单击此处 |
| `{{friendly_unsubscribe}}` | 厌倦了所有的邮件？ 请让我在这里知道 |
| `{{my_name}}` | 基思·弗林 |
| `{{my_signature}}` | Keith Flynn，Adobe高级技术撰稿人 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高级技术撰稿人 |
| `{{work_website}}` | https://www.adobe.com/cn |

**注意事项**：

* 如果联系人信息输入错误或从“人员”页面中丢失，则无法将联系人信息正确提取到您的模板中。
* `{{company}}`和`{{company_friendly}}`的区别在于`{{company_friendly}}`将从联系人的公司名称中删除任何正式标题，如Inc.、LLC.等。
* 使用`{{company_friendly}}`时，请确保在联系人详细信息中用逗号分隔Inc.或Co.。 这就是[!DNL Sales Insight Actions]在提取值时知道要移除内容的方式。
* 我们允许您使用预定义属性（如`{{my_name}}`或`{{my_title}}`）个性化电子邮件模板。 这些字段允许您在电子邮件模板中快速引用自己。
* 系统会自动将用户的签名附加到发送的每封电子邮件中。 如果用户使用包含`{{my_signature}}`动态字段的模板，系统将填充放置`{{my_signature}}`动态字段的签名。 只是为了避免重复而添加它。 启用全局附加取消订阅设置时，系统将以相同的方式处理`{{team_unsubscribe}}`。

>[!TIP]
>
>如果动态字段未填充，请查看[此文章](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md)。
