---
description: 动态字段 — Marketo文档 — 产品文档
title: 动态字段
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# 动态字段 {#dynamic-fields}

我们允许您使用预定义的属性(例如 `{{first_name}}` 或 `{{company}}`. 这些字段允许您向多个联系人发送电子邮件，并自动完成这些字段，而无需为每个联系人单独键入它们。

>[!TIP]
>
>“first_name”和“company”字段是仅有的将同时查看Sales Insight Actions和Salesforce的字段。 这意味着，如果联系人不存在于 [Web应用程序](https://toutapp.com/login)，我们会查看Salesforce以了解是否可以找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，使用该记录中的信息来填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在 **模板和营销活动**，找到要编辑的模板并单击 **编辑模板**.

1. 单击 **插入动态字段**.

   >[!NOTE]
   >
   >通过电子邮件发送存在于Sales Insight Actions中的联系人时，您可以使用基本的动态字段。 这些将直接从联系人中提取。

如果您通过电子邮件发送存在于Salesforce中的联系人，则可以利用Salesforce动态字段。 所有这些都以“sfdc”开头。 只要您连接到Salesforce，这些字段就会直接调用Salesforce中的潜在客户/联系人来填充模板中的信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，注意确保设置正确的格式。

## 动态字段默认值 {#dynamic-field-default-values}

将动态字段添加到电子邮件模板时，您可以添加一个默认值，如果没有其他可用值，动态字段将解析为该默认值。

为此，请在动态字段标签后添加“|”，然后添加“default：”（两者均不带引号）。 然后，如果找不到其他值，请添加您希望字段解析为的值（用引号括起来）。

**示例:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 动态字段术语表 {#dynamic-fields-glossary}

在Sales Insight Actions中创建模板时，我们始终建议使用 **插入动态字段** 按钮。

此工具用于 `auto-personalize your email` 为您节省大量时间 `pulling information from the People page`.

| 动态字段 | 电子邮件中显示内容示例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | 如果您不想再收到我们的电子邮件，请单击此处 |
| `{{friendly_unsubscribe}}` | 厌倦了所有的邮件？ 请让我在这里知道 |
| `{{my_name}}` | 基思·弗林 |
| `{{my_signature}}` | Keith Flynn，高级技术撰稿人 — Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高级技术撰稿人 |
| `{{work_website}}` | https://www.adobe.com |

**注意事项**：

* 如果联系人信息输入错误或从“人员”页面中丢失，则无法将联系人信息正确提取到您的模板中。
* 两者之间的差异 `{{company}}` 和 `{{company_friendly}}` 就是 `{{company_friendly}}` 将从您联系人的公司名称中删除任何正式标题，如Inc. 、 LLC等。
* 使用时 `{{company_friendly}}`，请确保在联系人详细信息中用逗号分隔Inc.或Co. 。 这就是Sales Insight Actions在提取值时知道要删除什么内容的方式。
* 我们允许您使用预定义的属性(例如 `{{my_name}}` 或 `{{my_title}}`. 这些字段允许您在电子邮件模板中快速引用自己。
* 系统会自动将用户的签名附加到发送的每封电子邮件中。 如果用户将模板与 `{{my_signature}}` 动态字段，系统将填充签名，其中 `{{my_signature}}` 已放置动态字段。 只是为了避免重复而添加它。 系统将处理 `{{team_unsubscribe}}` 与启用“全局附加取消订阅”设置时相同。

>[!TIP]
>
>如果动态字段未填充，请查看 [本文](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
