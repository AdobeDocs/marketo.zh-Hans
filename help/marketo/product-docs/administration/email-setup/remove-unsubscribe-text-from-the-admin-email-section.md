---
unique-page-id: 2360245
description: 从管理员电子邮件部分删除取消订阅文本 — Marketo文档 — 产品文档
title: 从管理员电子邮件部分删除取消订阅文本
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# 从“管理员”>“电子邮件”部分删除取消订阅文本 {#remove-unsubscribe-text-from-the-admin-email-section}

您应从&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Email]**&#x200B;区域完全删除取消订阅内容的唯一原因是，如果您选择在电子邮件模板中构建取消订阅链接。 该文本框具有验证，不允许您保存而不保存任何内容。 您可以通过添加小的HTML评论来解决此问题。 HTML注释将不会显示在电子邮件客户端中，因为它在HTML中呈现电子邮件，并且会忽略这些注释。 下面是操作方法。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. 选择所有文本并按&#x200B;**[!UICONTROL Delete]**&#x200B;键。

   >[!CAUTION]
   >
   >在删除之前，请将此文件作为备份复制/粘贴到文本文档中。

1. 键入`<!--This is a comment -->`。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. 单击 **[!UICONTROL Save Changes]**。

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>对于&#x200B;**取消订阅文本**，必须添加单个字符。 使用短划线或句点。
