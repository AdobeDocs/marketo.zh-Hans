---
unique-page-id: 1900585
description: 将可编辑部分添加到电子邮件模板v1.0 - Marketo文档 — 产品文档
title: 将可编辑部分添加到电子邮件模板v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 1%

---

# 将可编辑部分添加到电子邮件模板v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果您在电子邮件模板编辑器v1.0中创建模板，则可以通过添加特殊的 `<div>` 围着它。

>[!NOTE]
>
>**示例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

规则:

1. HTML必须始终有效。
1. 类 **mktEditable** 必须包括。
1. 该ID在该HTML中必须是唯一的。
1. ID中没有空格。

>[!CAUTION]
>
>无法嵌套mktEditable语句。

如果您想在电子邮件模板编辑器v2.0中了解如何执行此操作，请查看 [电子邮件模板语法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
