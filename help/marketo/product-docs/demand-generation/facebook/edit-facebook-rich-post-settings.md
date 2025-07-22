---
unique-page-id: 2950555
description: 编辑Facebook富帖子设置 — Marketo文档 — 产品文档
title: 编辑Facebook富帖子设置
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 编辑[!DNL Facebook]富帖子设置 {#edit-facebook-rich-post-settings}

当有人在[!DNL Facebook]上共享您时自定义帖子。

>[!AVAILABILITY]
>
>并非所有Marketo Engage用户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

Marketo _社交应用程序_&#x200B;允许您的潜在客户与其在Facebook、Twitter等社交网络上的连接共享您的登陆页面。 Facebook OpenGraph标记（OG标记）允许您指定将登陆页面中的哪些信息包含在Facebook帖子中。

## 选择富发布选项 {#select-rich-post-options}

您可以指定要在由共享从登陆页面生成的[!DNL Facebook]个丰富帖子中使用的页面信息类型。

1. 在编辑器中为&#x200B;***[!UICONTROL Facebook Message]**&#x200B;视频或社交按钮选择&#x200B;*[!DNL YouTube*]*。

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. 从[!DNL Facebook]消息的以下选项中进行选择。

   * 添加静态内容：选择此选项可手动输入标题、描述和描述。

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * 添加动态内容：您的社交应用可以使用登陆页面的`<TITLE>`、`<CAPTION>`和`<DESCRIPTION>`标记填充您的富文章。

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >这些标记应已存在于页面源中，但为了更好地控制，您可以向登陆页面添加特定的[!DNL Facebook] OG标记。

   * 不要添加丰富的内容：将登陆页面中的[!DNL Facebook]个帖子限制为仅添加主消息和链接。

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## 将[!DNL Facebook] OG标记添加到登陆页面 {#add-facebook-og-tags-to-a-landing-page}

要控制将从登陆页面包含在[!DNL Facebook]共享中的页面元素，您可以向登陆页面添加标题、描述和描述的[!DNL Facebook] OG （开放图形）标记。

1. 打开包含您的&#x200B;**[!DNL YouTube]视频**&#x200B;或社交按钮的登陆页面。

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   **[!UICONTROL Landing Page Designer]**&#x200B;将在新窗口中打开。

1. 选择&#x200B;**[!UICONTROL Landing Page Actions]** > **[!UICONTROL Edit Page Meta Tags]**。

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. 添加定义og:title、og:caption和og:description的HTML。 复制并粘贴这些行并替换占位符文本：

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>在添加OG标记时，请注意使用正确的HTML语法。
