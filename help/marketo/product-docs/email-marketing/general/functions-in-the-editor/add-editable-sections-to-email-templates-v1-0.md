---
unique-page-id: 1900585
description: 将可编辑部分添加到电子邮件模板v1.0 - Marketo Docs —— 产品文档
title: 将可编辑部分添加到电子邮件模板v1.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# 将可编辑部分添加到电子邮件模板v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果要在电子邮件模板编辑器v1.0中创建模板，则可以通过在其周围添加特殊内容来使任何部分 `<div>` 可编辑。

>[!NOTE]
>
>**示例**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

规则：

1. HTML必须始终有效。
1. 必须包 **含mktEditable** 类。
1. 该ID在该HTML中必须是唯一的。
1. ID中没有空格。

>[!CAUTION]
>
>mktEditable语句不能嵌套。

如果您想在“电子邮件模板编辑器v2.0”中了解如何执行此操作，请查看电子邮件 [模板语法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)。
