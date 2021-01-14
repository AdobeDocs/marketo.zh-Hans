---
unique-page-id: 2360245
description: 从“管理员电子邮件”部分删除取消订阅文本- Marketo文档——产品文档
title: 从“管理员电子邮件”部分删除取消订阅文本
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# 从管理员电子邮件部分{#remove-unsubscribe-text-from-the-admin-email-section}删除取消订阅文本

您应从“管理员>电子邮件”区域完全删除取消订阅内容的唯一原因是，您选择自己构建电子邮件模板中的取消订阅链接。 该文本框包含不允许保存内容的验证。 您可以通过添加小的HTML注释来解决此问题。 HTML注释不会显示在电子邮件客户端中，因为它以HTML格式呈现电子邮件，并且会忽略注释。 下面介绍如何实现。

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**电子邮件**。

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. 选择所有文本并按&#x200B;**Delete**&#x200B;键。

   >[!CAUTION]
   >
   >在删除之前，将其复制／粘贴到文本文档中作为备份。

1. 键入`<!--This is a comment -->`。

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. 单击&#x200B;**保存更改**。

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>对于&#x200B;**取消订阅文本**，您必须添加一个字符。 使用短划线或句点。
