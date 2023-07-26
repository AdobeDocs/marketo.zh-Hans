---
unique-page-id: 14352509
description: 动态字段术语表 — Marketo文档 — 产品文档
title: 动态字段术语表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 动态字段术语表 {#dynamic-fields-glossary}

在Sales Connect中创建模板时，我们始终建议使用 **MSE动态字段** 按钮。

此工具用于 `auto-personalize your email` 为您节省大量时间 `pulling information from the People page`.

| 动态字段 | 电子邮件中显示内容示例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | 如果你不想再听到我的消息，请让我知道 |
| `{{my_name}}` | 艾伦·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高级技术撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**注意事项**：

* 如果联系人信息输入错误或从“人员”页面中丢失，则无法将联系人信息正确提取到您的模板中。
* 两者之间的差异 `{{company}}` 和 `{{company_friendly}}` 就是 `{{company_friendly}}` 将从您联系人的公司名称中删除任何正式标题，如Inc. 、 LLC等。
* 使用时 `{{company_friendly}}`，请确保在联系人详细信息中用逗号分隔Inc.或Co. 。 这是Sales Connect在提取值时知道要移除什么内容的方法。

>[!TIP]
>
>您可以创建自己的 [自定义动态字段](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) 任何您想要自动提取到电子邮件中的内容
