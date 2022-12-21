---
unique-page-id: 1900573
description: 在电子邮件中添加系统令牌作为链接 — Marketo文档 — 产品文档
title: 在电子邮件中将系统令牌添加为链接
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# 在电子邮件中将系统令牌添加为链接 {#add-a-system-token-as-a-link-in-an-email}

您可以使用这些系统令牌来自定义特殊链接在电子邮件中的位置。

以下令牌可用作电子邮件或电子邮件模板中的链接：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>这些令牌将 **not** 可点击，除非在锚点链接中。 此外，他们还可以 **not** 嵌入到我的令牌中。

以下是如何将它们添加到电子邮件中：

1. 查找并选择您的电子邮件，然后单击 **编辑草稿**.

   ![](assets/one-1.png)

1. 在可编辑区域中双击。

   ![](assets/two-1.png)

1. 突出显示要转换为具有令牌的链接的文本，然后单击 **插入/编辑链接** 按钮。

   ![](assets/three-1.png)

1. 在链接URL中输入令牌，然后单击 **插入**.

   ![](assets/four-1.png)

   >[!TIP]
   >
   >复制/粘贴您需要的令牌： **`{{system.forwardToFriendLink}}`** 或 **`{{system.unsubscribeLink}}`** 或 **`{{system.viewAsWebpageLink}}`**

1. 单击 **保存**.

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>如果您使用此方法添加“viewAsWebpageLink”系统令牌，则可以 **not** 使用令牌覆盖它。 请改为使用 [将“查看为网页”链接添加到电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 方法，允许您使用令牌覆盖“viewAsWebPageLink”。

>[!NOTE]
>
>别忘了 [批准电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md) 完成时。

干得好！ 现在，您已了解如何在电子邮件中将系统令牌添加为链接。
