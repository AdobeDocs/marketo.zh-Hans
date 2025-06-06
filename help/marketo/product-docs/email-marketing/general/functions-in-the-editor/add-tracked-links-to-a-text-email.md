---
unique-page-id: 1900589
description: 将跟踪链接添加到文本电子邮件 — Marketo文档 — 产品文档
title: 将跟踪链接添加到文本电子邮件
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# 将跟踪链接添加到文本电子邮件 {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [创建纯文本电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [编辑电子邮件中的元素](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

可在Marketo中跟踪文本电子邮件链接。 让我们看看它是如何运作的。

1. 选择您的电子邮件并单击&#x200B;**编辑草稿**。

![](assets/one-9.png)

1. 双击要向其添加链接的可编辑区域。

   ![](assets/two-8.png)

1. 输入带有双括号的URL，如下所示： `[[www.domain.com/path/page.html]]`。

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >如果在365天前&#x200B;**和**&#x200B;发送了一封电子邮件，且过去180天内没有人点击过该电子邮件的任何链接，则Marketo Engage会从我们的数据库中修剪指向URL的路由，从而导致链接断开。 如果您需要永久性链接，请勿使用跟踪。

1. 关闭编辑器，别忘了批准草稿。

   ![](assets/four-6.png)

>[!NOTE]
>
>mktNoTok类功能不适用于文本电子邮件中的可跟踪链接。 仅适用于HTML电子邮件。
