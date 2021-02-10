---
unique-page-id: 1900573
description: 在电子邮件- Marketo Docs —— 产品文档中添加系统令牌作为链接
title: 将系统令牌添加为电子邮件中的链接
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---


# 在电子邮件{#add-a-system-token-as-a-link-in-an-email}中添加系统令牌作为链接

您可以使用这些系统令牌自定义特殊链接在电子邮件中的位置。

以下令牌可用作电子邮件或电子邮件模板中的链接：

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>这些令牌将&#x200B;**不**&#x200B;可单击，除非在锚点链接中。 而且，它们可以&#x200B;**不能**&#x200B;嵌入到我的令牌中。

下面介绍如何将它们添加到电子邮件：

1. 查找并选择您的电子邮件，然后单击&#x200B;**编辑草稿**。

   ![](assets/one-1.png)

1. 多次在可编辑区域中单击。

   ![](assets/two-1.png)

1. 高亮显示要转换为将包含令牌的链接的文本，然后单击&#x200B;**插入／编辑链接**&#x200B;按钮。

   ![](assets/three-1.png)

1. 在链接URL中输入令牌，然后单击&#x200B;**插入**。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >复制／粘贴所需的令牌：**`{{system.forwardToFriendLink}}`**&#x200B;或&#x200B;**`{{system.unsubscribeLink}}`**&#x200B;或&#x200B;**`{{system.viewAsWebpageLink}}`**

1. 单击&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!NOTE]
>
>完成后，不要忘记[批准电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)。

干得好！ 现在您了解如何将系统令牌添加为电子邮件中的链接。
