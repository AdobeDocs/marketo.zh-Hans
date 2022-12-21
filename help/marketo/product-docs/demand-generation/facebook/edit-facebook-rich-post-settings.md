---
unique-page-id: 2950555
description: 编辑Facebook富帖子设置 — Marketo文档 — 产品文档
title: 编辑Facebook富帖子设置
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# 编辑Facebook富帖子设置 {#edit-facebook-rich-post-settings}

在用户在Facebook上共享您时自定义帖子。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的销售代表。

Marketo [社交应用程序](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) 允许您的潜在客户在Facebook、Twitter等社交网络上与他们的连接共享您的登陆页面。 Facebook OpenGraph标记（OG标记）允许您指定登陆页面中的哪些信息包含在Facebook帖子中。

## 选择富帖子选项 {#select-rich-post-options}

您可以指定要在Facebook富帖子中使用的页面信息类型，这些帖子由从您的登陆页面共享生成。

1. 选择 **Facebook消息** 在 **YouTube** 视频或社交按钮。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 从以下选项中为您的Facebook消息选择。

   * 添加静态内容：选择此选项可手动输入标题、标题和描述。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 添加动态内容：您的社交应用程序可以使用登陆页面的 `<TITLE>`, `<CAPTION>`和 `<DESCRIPTION>` 标记来填充您的富帖子。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >这些标记应该已存在于页面源中，但要获得更多控制，您可以向登陆页面添加特定的Facebook OG标记。

   * 请勿添加富内容：将Facebook帖子从您的登陆页面限制为仅显示主消息和链接。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 将Facebook OG标记添加到登陆页面 {#add-facebook-og-tags-to-a-landing-page}

要控制将从登陆页面共享的Facebook中包含的页面元素，可以向登陆页面添加标题、描述和描述的Facebook OG(Open Graph)标记。

1. 打开包含您的 **YouTube视频** 或“社交”按钮。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   的 **登陆页面设计工具** 在新窗口中打开。

1. 选择 **登陆页面操作** > **编辑页面元标记**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 添加定义og:title、og:caption和og:description的HTML。 复制并粘贴这些行并替换占位符文本：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>添加OG标记时，请务必使用正确的HTML语法。
