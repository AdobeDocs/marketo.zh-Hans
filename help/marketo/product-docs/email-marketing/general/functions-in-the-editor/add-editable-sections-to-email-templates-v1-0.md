---
unique-page-id: 1900585
description: 向电子邮件模板v1.0 - Marketo文档 — 产品文档中添加可编辑的部分
title: 向电子邮件模板v1.0中添加可编辑的部分
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 1%

---

# 向电子邮件模板v1.0中添加可编辑的部分 {#add-editable-sections-to-email-templates-v1.0}

如果要在电子邮件模板编辑器v1.0中创建模板，则可以通过放置特殊的 `<div>` 周围。

>[!NOTE]
>
>**示例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

规则:

1. HTML必须始终有效。
1. 类 **mktEditable** 必须包含在内。
1. 该ID在该HTML中必须唯一。
1. ID中没有空格。

>[!CAUTION]
>
>无法嵌套mktEditable语句。

如果您想要了解如何在电子邮件模板编辑器v2.0中执行此操作，请参阅 [电子邮件模板语法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
