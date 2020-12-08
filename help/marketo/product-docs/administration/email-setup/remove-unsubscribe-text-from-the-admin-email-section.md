---
unique-page-id: 2360245
description: 从“管理员->电子邮件”部分- Marketo Docs —— 产品文档中删除取消订阅文本
title: 从“管理员->电子邮件”部分删除取消订阅文本
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# 从“管理员->电子邮件”部分删除取消订阅文本 {#remove-unsubscribe-text-from-the-admin-email-section}

您应从“管理员>电子邮件”区域完全删除取消订阅内容的唯一原因是，您选择自己构建电子邮件模板中的取消订阅链接。 该文本框包含不允许保存内容的验证。 您可以通过添加小的HTML注释来解决此问题。 HTML注释不会显示在电子邮件客户端中，因为它以HTML格式呈现电子邮件，并且会忽略注释。 下面介绍如何实现。

1. 转到“管 **理员** ”并单 **击“电子邮件**”。

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. 选择所有文本并按**Delete **键。

   >[!CAUTION]
   >
   >在删除之前，将其复制／粘贴到文本文档中作为备份。

1. 输入 **<!--This is a comment -->**。

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. 单击“ **保存更改**”。

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>对于**取消订阅文本**，您必须添加一个字符。 使用短划线或句点。

