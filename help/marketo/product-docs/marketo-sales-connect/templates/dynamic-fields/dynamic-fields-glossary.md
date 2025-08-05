---
unique-page-id: 14352509
description: 动态字段术语表 — Marketo文档 — 产品文档
title: 动态字段术语表
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# 动态字段术语表 {#dynamic-fields-glossary}

在[!DNL Sales Connect]中创建模板时，我们始终建议使用&#x200B;**[!UICONTROL MSE Dynamic Fields]**&#x200B;按钮集成动态字段。

此工具用于`auto-personalize your email`，并由`pulling information from the [!UICONTROL People] page`为您节省大量时间。

| 动态字段 | 电子邮件中显示内容示例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | 如果您不想再收到我们的电子邮件，请单击此处 |
| `{{friendly_unsubscribe}}` | 厌倦了所有的邮件？ 请让我在这里知道 |
| `{{my_name}}` | 基思·弗林 |
| `{{my_signature}}` | Keith Flynn，Adobe高级技术撰稿人 |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | 高级技术撰稿人 |
| `{{work_website}}` | <https://www.adobe.com> |

**注意事项**：

* 如果联系人信息输入错误或从“人员”页面中丢失，则无法将联系人信息正确提取到您的模板中。
* `{{company}}`和`{{company_friendly}}`的区别在于`{{company_friendly}}`将从联系人的公司名称中删除任何正式标题，如Inc.、LLC.等。
* 使用`{{company_friendly}}`时，请确保在联系人详细信息中用逗号分隔Inc.或Co.。 这是Sales Connect在提取值时知道要移除什么内容的方法。
* 系统会自动将用户的签名附加到发送的每封电子邮件中。 如果用户使用包含`{{my_signature}}`动态字段的模板，系统将填充放置`{{my_signature}}`动态字段的签名。 只是为了避免重复而添加它。 启用全局附加取消订阅设置时，系统将以相同的方式处理`{{team_unsubscribe}}`。

>[!TIP]
>
>您可以为要自动提取到电子邮件中的任何内容创建自己的[自定义动态字段](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)
