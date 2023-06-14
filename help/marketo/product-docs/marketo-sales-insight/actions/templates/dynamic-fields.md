---
description: 动态字段 — Marketo文档 — 产品文档
title: 动态字段
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: 6d4a093d0ce0158028177cc4a4088526ccf79f9d
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 动态字段 {#dynamic-fields}

我们允许您使用预定义的属性对电子邮件模板进行个性化设置，例如 `{{first_name}}` 或 `{{company}}`. 这些字段允许您向多个联系人发送电子邮件，并自动完成这些字段，而无需为每个联系人单独键入它们。

>[!TIP]
>
>“first_name”和“company”字段是仅有的两个将同时查看Sales Insight Actions和Salesforce的字段。 这意味着如果联系人不存在于 [Web应用程序](https://toutapp.com/login)，我们会查看Salesforce以了解是否可以找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，我们使用该记录中的信息填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. In **模板和营销活动**，找到要编辑的模板并单击 **编辑模板**.

1. 单击 **插入动态字段**.

   >[!NOTE]
   >
   >通过电子邮件发送存在于Sales Insight Actions中的联系人时，您可以使用基本的动态字段。 这些将直接从联系人中提取。

如果您通过电子邮件发送存在于Salesforce中的联系人，则可以利用Salesforce动态字段。 所有这些都以“sfdc”开头。 只要您连接到Salesforce，这些字段就会直接调用Salesforce中的潜在客户/联系人，以在模板中填充信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，注意确保设置正确的格式。

## 动态字段默认值 {#dynamic-field-default-values}

将动态字段添加到电子邮件模板时，您可以添加一个默认值，如果没有其他可用值，动态字段将解析为该默认值。

为此，请在动态字段标签后添加“|”，然后添加“default：”（两者均不带引号）。 然后，如果找不到其他值，请添加您希望字段解析为（用引号括起来）的值。

**示例：**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 动态字段术语表 {#dynamic-fields-glossary}

在Sales Insight Actions中创建模板时，我们始终建议使用 **插入动态字段** 按钮。

此工具用于 `auto-personalize your email` 为您节省大量时间，方法是 `pulling information from the People page`.

| 动态字段 | 电子邮件中显示的内容示例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | 如果你不想再收到我的信，请通知我 |
| `{{my_name}}` | 艾伦·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高级技术撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**注意事项**：

* 如果联系人信息输入错误或从“人员”页面中丢失，则无法将信息正确提取到模板中。
* 两者之间的差异 `{{company}}` 和 `{{company_friendly}}` 就是 `{{company_friendly}}` 将从您联系人的公司名称中删除任何正式名称，如Inc.、LLC.等。
* 使用时 `{{company_friendly}}`，请确保在联系人详细信息中用逗号分隔Inc.或Co.。 这就是Sales Insight Actions在提取值时知道要移除什么内容的方式。
* 我们允许您使用预定义的属性对电子邮件模板进行个性化设置，例如 `{{my_name}}` 或 `{{my_title}}`. 这些字段允许您在电子邮件模板中快速引用自己。

>[!TIP]
>
>如果动态字段未填充，请查看 [本文](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
