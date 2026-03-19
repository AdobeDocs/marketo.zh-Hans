---
unique-page-id: 1900585
description: 了解如何在v1.0中将可编辑部分添加到电子邮件模板。允许用户编辑特定区域，同时保持其余区域处于锁定状态。
title: 向电子邮件模板 v1.0 添加可编辑部分
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 13%

---

# 向电子邮件模板 v1.0 添加可编辑部分 {#add-editable-sections-to-email-templates-v1.0}

如果您在电子邮件模板编辑器v1.0中创建模板，则可以通过在任意部分周围放置特殊`<div>`来使其可编辑。

>[!NOTE]
>
>**示例**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

规则：

1. HTML必须始终有效。
1. 必须包括&#x200B;**mktEditable**&#x200B;类。
1. 该ID在该HTML中必须是唯一的。
1. ID中没有空格。

>[!CAUTION]
>
>无法嵌套mktEditable语句。

如果要在电子邮件模板编辑器v2.0中了解如何执行此操作，请查看[电子邮件模板语法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)。
