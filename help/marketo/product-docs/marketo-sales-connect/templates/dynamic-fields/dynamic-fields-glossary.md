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


# 动态字段词汇表 {#dynamic-fields-glossary}

在Sales Connect中创建模板时，我们始终建议使用“MSE动态字段”按 **钮集成动态字段** 。

此工具可 `auto-personalize your email` 以帮您节省大量时间 `pulling information from the People page`。

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

* 如果联系人的 `information is entered incorrectly` 或在“人员”页面中缺失，则该联系人 `will not pull over correctly` 会进入模板。

* 不同之 `{{company}}` 处 `{{company_friendly}}` 在于， `{{company_friendly}}``remove any formal title`将（如Inc.、 LLC等）从您联系人的公司名称中删除。
* 使用时， `{{company_friendly}}`请确保在联系人详细信息中以逗号分隔Inc.或Co.。 这就是Sales Connect在提取值时如何删除的方法。

>[!TIP]
>
>您可以为想要自动 [加入电子邮件](http://docs.marketo.com/x/fADb) ，创建您自己的自定义动态字段

