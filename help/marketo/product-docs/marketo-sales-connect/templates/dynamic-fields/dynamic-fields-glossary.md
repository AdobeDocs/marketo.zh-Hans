---
unique-page-id: 14352509
description: 动态字段词汇表- Marketo Docs —— 产品文档
title: 动态字段词汇表
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---


# 动态字段术语表{#dynamic-fields-glossary}

在Sales Connect中创建模板时，我们始终建议使用&#x200B;**MSE Dynamic Fields**&#x200B;按钮集成动态字段。

此工具用于`auto-personalize your email`并通过`pulling information from the People page`节省大量时间。

| 动态字段 | 电子邮件中显示的示例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | 基思 |
| `{{friendly_unsubscribe}}` | 如果你不想再听我的，请告诉我 |
| `{{my_name}}` | 艾伦·布拉德利 |
| `{{personal_email}}` | [[电子邮件受保护]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | 高级技术作者 |
| `{{work_website}}` | https://www.marketo.com |

**注意事项**:

* 如果联系人的`information is entered incorrectly`或“人员”页面中缺少联系人，则该联系人`will not pull over correctly`将进入您的模板。

* `{{company}}`和`{{company_friendly}}`之间的区别在于，`{{company_friendly}}`将从联系人的公司名称中`remove any formal title`（如Inc.、LLC等）。
* 使用`{{company_friendly}}`时，请确保在联系人详细信息中以逗号分隔Inc.或Co.。 这就是Sales Connect在提取值时如何删除的方法。

>[!TIP]
>
>您可以为想要自动添加到电子邮件中的任何内容创建自己的[自定义动态字段](http://docs.marketo.com/x/fADb)

