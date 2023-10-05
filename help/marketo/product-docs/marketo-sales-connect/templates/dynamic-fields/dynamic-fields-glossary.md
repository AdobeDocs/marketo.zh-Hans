---
unique-page-id: 14352509
description: 动态字段术语表 — Marketo文档 — 产品文档
title: 动态字段术语表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# 动态字段术语表 {#dynamic-fields-glossary}

在Sales Connect中创建模板时，我们始终建议使用 **MSE动态字段** 按钮。

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
* 使用时 `{{company_friendly}}`，请确保在联系人详细信息中用逗号分隔Inc.或Co. 。 这是Sales Connect在提取值时知道要移除什么内容的方法。
* 如果您使用 `{{my_signature}}` 动态字段，系统将不会自动附加用户的签名以防止重复。

>[!TIP]
>
>您可以创建自己的 [自定义动态字段](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) 任何您想要自动提取到电子邮件中的内容
