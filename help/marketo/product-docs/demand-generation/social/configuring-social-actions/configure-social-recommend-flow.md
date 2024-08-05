---
unique-page-id: 2950549
description: 配置社交推荐流程 — Marketo文档 — 产品文档
title: 配置社交推荐流程
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 配置社交推荐流程 {#configure-social-recommend-flow}

在创建社交应用程序时，您可以配置社交网络选项，并在用户注册时提示用户遇到这些选项。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 您将无法创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## 选择要共享的网络 {#select-networks-for-sharing}

>[!NOTE]
>
>这与[配置社交注册/共享流](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md)非常相似，但这适用于社交应用程序&#x200B;_下的共享链接_。

1. 转到&#x200B;**营销活动**。

   ![](assets/login-marketing-activities-1.png)

1. 选择应用程序，然后单击&#x200B;**编辑草稿**。

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. 在社交应用编辑器中，转到&#x200B;**建议流** > **社交网络**。

   ![](assets/recommendedflow.png)

1. 选择用户可以共享到的网络。

   ![](assets/socialnetworkschoose.png)

## 配置Facebook消息 {#configure-the-facebook-message}

1. 配置将显示在Facebook帖子中的消息。

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >在视频共享中，会自动生成缩略图。

   如果选择&#x200B;**添加动态内容**，则页面的OpenGraph标记（og：title、og：caption和og：description）和缩览图的值将自动添加到Facebook帖子中。 查看下一步。

   如果选择&#x200B;**添加静态内容**，请输入标题、题注和描述，然后上传图像。 查看接下来的两个步骤。

1. 在“查看和编辑”窗口中，单击&#x200B;**显示编辑**&#x200B;以自定义将显示在Facebook帖子中的共享提示和消息。

   >[!TIP]
   >
   >有关详细信息，请参阅[编辑Facebook富媒体帖子设置](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md)。

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >[共享URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)已自动添加到所有共享消息中。

1. 如果选择上述&#x200B;**添加静态内容**，请编辑标题、标题和描述，并上传自定义图像(从Marketo图像和文件)。

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   请参阅[将图像和文件添加到Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)。

   >[!NOTE]
   >
   >如果上传图像，则直到关闭并重新打开社交应用程序编辑器后，您才会在此处看到该图像。

1. 单击&#x200B;**下一步**。

如果选择，则页面的OpenGraph标记（og：title、og：caption和og：description）和缩略图的值将自动添加到Facebook帖子中。 请参阅下一步。

## 配置Twitter消息 {#configure-the-twitter-message}

1. 单击可编辑共享提示和将显示在Twitter推文中的消息。

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >在推文文本中使用{html_title}自动显示页面标题。

1. 单击&#x200B;**下一步**。

## 配置LinkedIn消息 {#configure-the-linkedin-message}

1. 配置将显示在LinkedIn帖子中的消息。

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   如果选择&#x200B;**添加动态**&#x200B;内容，则页面标记的值（标题和描述）以及缩览图将自动添加到LinkedIn帖子中。 查看下一步。

   如果选择&#x200B;**添加静态**&#x200B;内容，请输入标题、题注和描述，然后上传图像。 查看接下来的两个步骤。

1. 在&#x200B;**查看并编辑**&#x200B;窗口中，单击&#x200B;**显示编辑**&#x200B;并编辑将显示在LinkedIn帖子中的共享提示和消息。

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >在帖子文本中使用{html_title}自动显示页面的标题。

1. 如果选择了&#x200B;**“添加静态**&#x200B;内容”，请编辑标题和描述，并(从Marketo图像和文件)上传自定义图像。

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   请参阅[将图像和文件添加到Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)。

   >[!NOTE]
   >
   >如果上传图像，则直到关闭并重新打开社交应用程序编辑器后才会在此处看到该图像。

1. 单击&#x200B;**下一步**。

## 配置确认消息 {#configure-the-confirmation-message}

1. 编辑共享确认文本。

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. 单击&#x200B;**完成** > **批准**&#x200B;和&#x200B;**关闭**。

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>下一步是[将您的视频共享](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md)或[轮询](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md)添加到登陆页、Facebook或您自己的网站。
