---
unique-page-id: 2950524
description: 在网站上部署Social - Marketo文档 — 产品文档
title: 在您的网站上部署Social
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 在您的网站上部署Social {#deploy-social-on-your-website}

在非Marketo页面上嵌入社交应用程序。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 无法再创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>并非所有Marketo Engage用户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

您可以在自己的网站上部署社交应用程序，以吸引受众，并使每个人都参与社交网络上的大型对话。 当人们在社交网络上与好友共享您的促销活动和内容时，您会在网站上生成更多流量。

1. 选择批准的社交应用程序，如YouTube视频或社交按钮。

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. 从社交应用程序操作中选择&#x200B;**嵌入代码**。

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. 复制网站页眉(`<head>`)和正文(`<body>`)的代码。

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. 将第一个代码段粘贴到网站的页眉中。

   ![](assets/socialonsite-embedhead.png)

1. 将第二个代码段粘贴到每个页面中，您希望您的社交应用程序显示在页面中的位置。

   ![](assets/socialonsite-embedwidget.png)

1. 如果需要将社交应用程序的大小设置为页面上的特定维度，请将&#x200B;**outerHeight**&#x200B;和&#x200B;**outerWidth**&#x200B;选项添加到第二个代码片段中。 例如，您可以添加`options='{"outerHeight":400, "outerWidth":600}'`，如下所示：

   ![](assets/socialonsite-resizewidget2.png)

   您的Marketo社交应用程序现在为网站添加内容和交互性，邀请粉丝、访客和现有客户传播有关您的信息。 同时，它还将其用户档案数据添加到您的数据库并跟踪社交影响指标。

   >[!MORELIKETHIS]
   >
   >* [自定义社交应用按钮](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [设置社交共享要求](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish登录页面到Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
