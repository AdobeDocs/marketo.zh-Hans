---
unique-page-id: 1900585
description: 将可编辑部分添加到电子邮件模板v1.0 - Marketo Docs —— 产品文档
title: 将可编辑部分添加到电子邮件模板v1.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# 将可编辑部分添加到电子邮件模板v1.0 {#add-editable-sections-to-email-templates-v1.0}

如果要在电子邮件模板编辑器v1.0中创建模板，则可以通过在其周围放置一个特殊的`<div>`来使任何部分都可编辑。

>[!NOTE]
>
>**示例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

规则：

1. HTML必须始终有效。
1. 必须包括&#x200B;**mktEditable**&#x200B;的类。
1. 该ID在该HTML中必须是唯一的。
1. ID中没有空格。

>[!CAUTION]
>
>mktEditable语句不能嵌套。

如果要在电子邮件模板编辑器v2.0中了解如何执行此操作，请查看[电子邮件模板语法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)。
