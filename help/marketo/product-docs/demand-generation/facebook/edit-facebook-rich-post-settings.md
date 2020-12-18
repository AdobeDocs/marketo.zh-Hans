---
unique-page-id: 2950555
description: 编辑Facebook富帖子设置——营销文档——产品文档
title: 编辑Facebook富帖子设置
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# 编辑Facebook富帖子设置{#edit-facebook-rich-post-settings}

当用户[在Facebook上共享您](http://docs.marketo.com/display/docs/social)时自定义帖子。

>[!NOTE]
>
>**可用性**
>
>并非所有客户都购买了此功能。 有关详细信息，请与销售代表联系。

Marketo [社交应用程序](http://docs.marketo.com/display/docs/social)允许您的潜在客户在Facebook、Twitter等社交网络上与其连接共享登陆页。 Facebook OpenGraph标记（OG标记）允许您指定Facebook帖子中包含来自登陆页的信息。

## 选择富发布选项{#select-rich-post-options}

您可以指定要在Facebook富帖子中使用的页面信息类型，这些帖子由您的登陆页共享生成。

1. 在编辑器中选择&#x200B;**YouTube**&#x200B;视频或社交按钮的&#x200B;**Facebook消息**。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 从以下选项中选择您的Facebook消息。

   * 添加静态内容：选择此选项可手动输入标题、题注和说明。

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 添加动态内容：您的社交应用程序可以使用登陆页的`<TITLE>`、`<CAPTION>`和`<DESCRIPTION>`标记填充您的丰富帖子。

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >页面源中应已存在这些标记，但要获得更多控制，您可以[向登陆页添加特定Facebook OG标记](edit-facebook-rich-post-settings.md)。

   * 不添加丰富内容：将Facebook帖子从您的登陆页限制为仅主要消息和链接。

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## 向登陆页{#add-facebook-og-tags-to-a-landing-page}添加Facebook OG标记

要控制将包含在您的登陆页的Facebook共享中的页面元素，可以向登陆页添加标题、题注和说明的Facebook OG(Open Graph)标记。

1. 打开包含&#x200B;**YouTube视频**&#x200B;或社交按钮的登陆页。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **登陆页设计器**&#x200B;在新窗口中打开。

1. 选择&#x200B;**登陆页操作** > **编辑页面元标记****.**

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 添加定义og:title、og:caption和og:description的HTML。 复制并粘贴这些行并替换占位符文本：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>添加OG标记时，请注意使用正确的HTML语法。
