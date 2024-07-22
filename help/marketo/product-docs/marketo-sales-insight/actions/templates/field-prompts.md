---
description: 字段提示 — Marketo文档 — 产品文档
title: 字段提示
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# 字段提示 {#field-prompts}

利用字段提示，可以向需要删除或替换的电子邮件添加文本字符串，然后才能发送电子邮件。 这是提醒用户添加其他个性化的绝佳方式。

要添加字段提示，请键入所需的文本。 在开头使用感叹号，并在前面加上大括号（见下文）。

**示例：**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>在发送电子邮件之前，用户需要用他们自己的个性化替换此文本。

![](assets/field-prompts-1.png)

>[!NOTE]
>
>在促销活动中使用提示时，最好将它们与手动电子邮件步骤结合使用。 这些步骤将为用户分配一个提醒任务来发送电子邮件，使他们有机会将提示替换为自定义文本。 Sales Campaigns中的自动电子邮件步骤将尝试自动发送，不允许用户替换提示。 未替换的提示将导致电子邮件发送失败。
