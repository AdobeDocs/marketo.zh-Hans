---
unique-page-id: 2950530
description: 配置社交注册/共享流程 — Marketo文档 — 产品文档
title: 配置社交注册/共享流
exl-id: 521187d1-2228-42e7-a87b-3b20a45adb03
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# 配置社交注册/共享流 {#configure-social-sign-up-share-flow}

在创建社交应用程序时，您可以配置社交网络选项，并在用户注册时提示用户遇到这些选项。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 无法再创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 选择要共享的网络 {#select-networks-for-sharing}

1. 转到&#x200B;**营销活动**。

   ![](assets/ma-1.png)

1. 选择应用程序，然后单击&#x200B;**编辑草稿**。

   ![](assets/image2014-9-22-13-3a57-3a43.png)

1. 在社交应用编辑器中，单击&#x200B;**注册流程** > **社交网络**。

   ![](assets/three.png)

1. 选择（或取消选择）人员可以共享到的网络。

   ![](assets/four.png)

## 配置Facebook消息 {#configure-the-facebook-message}

1. 转到&#x200B;**注册流程** > **共享邮件**。

   ![](assets/five.png)

1. 配置将显示在Facebook帖子中的消息。

   ![](assets/image2014-9-22-13-3a58-3a54.png)

   >[!NOTE]
   >
   >在视频共享中，将自动生成缩略图。

   如果选择&#x200B;**添加动态内容**，则页面的&#x200B;**OpenGraph**&#x200B;标记（og：title、og：caption和og：description）和缩略图的值将自动添加到Facebook帖子中。 请参阅下一步。

   如果选择&#x200B;**添加静态内容**，请输入标题、标题、描述并上传图像。 请参阅下面的两个步骤。

1. 在“查看和编辑”窗口中，单击&#x200B;**显示编辑内容**&#x200B;并编辑共享提示和将显示在Facebook帖子中的消息。

   >[!TIP]
   >
   >有关详细信息，请参阅[编辑Facebook富帖子设置](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md)。

   ![](assets/image2014-9-22-13-3a59-3a57.png)

   >[!NOTE]
   >
   >[共享URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)已自动添加到所有共享消息中。

1. 如果选择上述&#x200B;**添加静态内容**，请编辑标题、标题和描述，并上传自定义图像(来自&#x200B;[**Marketo图像和文件**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md))。

   ![](assets/image2014-9-22-14-3a1-3a11.png)

   请参阅[将图像和文件添加到Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)。

   >[!NOTE]
   >
   >如果上传图像，则直到关闭并重新打开社交应用程序编辑器后，您才会在此处看到该图像。

1. 单击&#x200B;**下一步**。

如果您选择页面标签的值（og：title、og：caption和og：description），则缩略图会自动添加到Facebook帖子中。 请参阅下一步。

## 配置Twitter消息 {#configure-the-twitter-message}

1. 编辑共享提示和将显示在Twitter推文中的消息。

   ![](assets/image2014-9-22-14-3a2-3a31.png)

   >[!TIP]
   >
   >在推文文本中使用{html_title}自动显示页面标题。

1. 单击&#x200B;**下一步**。

## 配置LinkedIn消息 {#configure-the-linkedin-message}

1. 配置将显示在LinkedIn帖子中的消息。

   ![](assets/image2014-9-22-14-3a3-3a8.png)

   如果选择&#x200B;**添加动态内容**，则页面标记的值（标题和描述）以及缩略图会自动添加到LinkedIn帖子中。 请参阅下一步。

   如果选择&#x200B;**添加静态内容**，请输入标题、标题和描述，然后上载图像。 请参阅下面的两个步骤。

1. 在&#x200B;**查看和编辑**&#x200B;窗口中，单击&#x200B;**显示编辑内容**&#x200B;并编辑共享提示和将显示在LinkedIn帖子中的消息。

   ![](assets/image2014-9-22-14-3a4-3a6.png)

   >[!TIP]
   >
   >在您的帖子文本中使用{html_title}自动显示页面标题。

1. 如果您选择了上面的&#x200B;**添加静态内容**，请编辑标题和描述，并上传自定义图像(从&#x200B;[**Marketo图像和文件**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md))。

   ![](assets/image2014-9-22-13-3a55-3a17.png)

>[!NOTE]
>
>如果上传图像，则直到关闭并重新打开社交应用程序编辑器后，您才会在此处看到该图像。

>[!MORELIKETHIS]
>
>接下来，您可以单击&#x200B;**完成** > **批准并关闭**，并将您的社交应用程序置于登陆页面上。 您还可以配置[人员捕获](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-person-capture-for-a-social-app.md)或[重新共享提示](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-re-share-email-and-prompt-for-a-social-app.md)。
