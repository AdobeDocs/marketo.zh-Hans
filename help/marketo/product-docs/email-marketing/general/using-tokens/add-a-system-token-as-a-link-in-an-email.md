---
unique-page-id: 1900573
description: 添加系统令牌作为电子邮件中的链接 — Marketo文档 — 产品文档
title: 添加系统令牌作为电子邮件中的链接
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 添加系统令牌作为电子邮件中的链接 {#add-a-system-token-as-a-link-in-an-email}

您可以使用这些系统令牌来自定义特殊链接在电子邮件中的位置。

以下令牌可用作电子邮件或电子邮件模板中的链接：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>除非位于锚点链接内部，否则这些令牌将&#x200B;**无法**&#x200B;点击。 此外，它们&#x200B;**不能**&#x200B;嵌入到“我的令牌”中。

以下是如何将它们添加到电子邮件中的：

1. 查找并选择您的电子邮件，然后单击&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/one-1.png)

1. 在可编辑区域中双击。

   ![](assets/two-1.png)

1. 突出显示要转换为具有令牌的链接的文本，然后单击&#x200B;**[!UICONTROL Insert/Edit Link]**&#x200B;按钮。

   ![](assets/three-1.png)

1. 在链接URL中输入令牌并单击&#x200B;**[!UICONTROL Insert]**。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >复制/粘贴所需的令牌： **`{{system.forwardToFriendLink}}`**、**`{{system.unsubscribeLink}}`**&#x200B;或&#x200B;**`{{system.viewAsWebpageLink}}`**

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>如果您使用此方法添加“viewAsWebPageLink”系统令牌，则&#x200B;**不能**&#x200B;使用令牌覆盖它。 请改为使用[将视图作为网页链接添加到电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)方法，此方法允许您使用令牌覆盖“viewAsWebPageLink”。

>[!NOTE]
>
>完成时，不要忘记[批准您的电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)。

做得好！ 现在您知道如何在电子邮件中添加系统令牌作为链接了。
