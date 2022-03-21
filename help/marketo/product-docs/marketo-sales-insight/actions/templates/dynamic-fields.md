---
description: 动态字段 — Marketo文档 — 产品文档
title: 动态字段
hide: true
hidefromtoc: true
source-git-commit: a0b10255513c13b7100b667513e3e61fc3788a15
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 动态字段 {#dynamic-fields}

我们允许您使用诸如之类的预定义属性来个性化电子邮件模板 `{{first_name}}` 或 `{{company}}`. 这些字段允许您通过电子邮件发送多个联系人并自动填写这些字段，而无需为每个联系人单独键入这些字段。

>[!TIP]
>
>“first_name”和“company”字段是唯一同时考虑Sales Insight Actions和Salesforce的字段。 这意味着如果 [Web应用程序](https://toutapp.com/login)，我们会在Salesforce中查看我们是否可以找到具有匹配电子邮件地址的联系人/潜在客户记录。 然后，我们使用该记录中的信息来填充该字段。

## 将动态字段插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在 **模板和营销活动**，找到要编辑的模板并单击 **编辑模板**.

1. 单击 **插入动态字段**.

   >[!NOTE]
   >
   >向Sales Insight Actions中存在的联系人发送电子邮件时，您可以使用基本的动态字段。 这些将直接从联系人处获取。

如果您向Salesforce中存在的联系人发送电子邮件，则可以利用Salesforce动态字段。 这些都以“sfdc”开头。 只要您与Salesforce建立连接，这些字段就会直接致电Salesforce中的潜在客户/联系人，以填充模板中的信息。

## 在主题行中插入动态字段 {#insert-dynamic-fields-in-a-subject-line}

只需手动将它们复制并粘贴到电子邮件的主题字段中，请务必确保格式正确。

## 动态字段术语表 {#dynamic-fields-glossary}

在Sales Insight Actions中创建模板时，我们始终建议使用 **插入动态字段** 按钮。

此工具用于 `auto-personalize your email` 省下大量时间 `pulling information from the People page`.

| 动态字段 | 电子邮件中显示的内容示例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | 基斯 |
| `{{friendly_unsubscribe}}` | 如果你不想再听我的话，请告诉我 |
| `{{my_name}}` | 艾伦·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高级技术作家 |
| `{{work_website}}` | https://www.marketo.com |

**注意事项**:

* 如果联系人的信息输入错误或在“人员”页面中缺失，则该信息无法正确提取到您的模板中。
* 两者之间的差异 `{{company}}` 和 `{{company_friendly}}` 是 `{{company_friendly}}` 将从联系人的公司名称中删除任何正式标题，如Inc.、 LLC等。
* 使用 `{{company_friendly}}`，请确保在联系详细信息中使用逗号分隔Inc.或Co.。 这就是Sales Insight Actions在提取值时如何删除内容的方式。
* 我们允许您使用诸如之类的预定义属性来个性化电子邮件模板 `{{my_name}}` 或 `{{my_title}}`. 利用这些字段，可在电子邮件模板中快速引用自己。

>[!TIP]
>
>如果动态字段未填充，请签出 [本文](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
