---
unique-page-id: 2360245
description: 从管理员电子邮件部分 — Marketo文档 — 产品文档中删除取消订阅文本
title: 从管理员电子邮件部分删除取消订阅文本
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 从管理员电子邮件部分删除取消订阅文本 {#remove-unsubscribe-text-from-the-admin-email-section}

您之所以应从“管理员>电子邮件”区域完全删除取消订阅内容，唯一的原因是您选择自行构建电子邮件模板中的取消订阅链接。 文本框包含的验证不允许您保存而不包含任何内容。 您可以通过添加一个小的HTML注释来解决此问题。 HTML评论将不会显示在电子邮件客户端中，因为它将以HTML方式呈现电子邮件，并且会忽略评论。 这是如何做到的。

1. 转到 **管理员** 的上界。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 单击 **电子邮件**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. 选择所有文本，然后按 **删除** 键。

   >[!CAUTION]
   >
   >在删除之前，将其复制/粘贴到文本文档中作为备份。

1. 键入 `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 单击 **保存更改**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>对于 **取消订阅文本** 您必须添加单个字符。 使用短划线或句点。
