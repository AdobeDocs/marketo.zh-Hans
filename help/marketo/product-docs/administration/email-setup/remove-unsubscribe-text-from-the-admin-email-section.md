---
unique-page-id: 2360245
description: 从管理员电子邮件部分删除取消订阅文本 — Marketo文档 — 产品文档
title: 从“管理员电子邮件”部分删除取消订阅文本
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# 从“管理员电子邮件”部分删除取消订阅文本 {#remove-unsubscribe-text-from-the-admin-email-section}

您应完全从 **[!UICONTROL 管理员]** > **[!UICONTROL 电子邮件]** 区域是指，如果您选择将取消订阅链接构建到电子邮件模板本身。 文本框验证不允许您保存而不保存任何内容。 您可以通过添加小型HTML评论来解决此问题。 HTML注释将不会显示在电子邮件客户端中，因为它以HTML呈现电子邮件，并且忽略这些注释。 下面是操作方法。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 单击 **[!UICONTROL 电子邮件]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. 选择所有文本并按 **[!UICONTROL 删除]** 键。

   >[!CAUTION]
   >
   >在删除之前，请将此文件作为备份复制/粘贴到文本文档中。

1. 键入 `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 单击 **[!UICONTROL 保存更改]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>对于 **取消订阅文本** 必须添加单个字符。 使用短划线或句点。
