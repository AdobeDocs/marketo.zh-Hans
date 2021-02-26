---
unique-page-id: 10092925
description: 预览和测试Web活动- Marketo Docs — 产品文档
title: 预览和测试Web活动
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# 预览和测试Web活动{#preview-and-test-a-web-campaign}

本文向您介绍了预览Web活动的不同方法，以及如何使用网站上实时的沙箱段对其进行测试。

## 预览创建页面{#preview-a-web-campaign-on-the-creation-page}上的Web活动

1. 转到&#x200B;**Web活动**。

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. 单击&#x200B;**“新建Web活动”**&#x200B;或图标以编辑现有活动。

   ![](assets/create-new-or-edit-web-campaign.png)

1. 在站点上的预览中，添加页面URL并单击&#x200B;**预览**。 将打开一个新窗口/选项卡，其中显示活动预览。

   ![](assets/three-1.png)

   >[!TIP]
   >
   >单击&#x200B;**共享**&#x200B;以打开包含活动预览固定URL的电子邮件。

   >[!NOTE]
   >
   >您还可以选择安装浏览器插件（[Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj)或[Firefox](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)），以获得预览活动的最佳体验。 请参阅下面的部分。

## 使用浏览器插件{#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}在创建页面上预览Web活动

1. 请遵循上面部分中的步骤1和2。

1. 单击指向浏览器插件的链接（在本例中，我们使用的是Chrome）。

   ![](assets/4-1.png)

1. 将打开新窗口/选项卡。 单击&#x200B;**添加到Chrome**。

   ![](assets/five.png)

1. 单击&#x200B;**添加扩展**。

   ![](assets/six.png)

1. 回马克托。 添加页面URL，然后单击&#x200B;**预览**。

   ![](assets/seven.png)

1. 此时会打开一个新窗口/选项卡，用于预览活动在桌面、手机或平板电脑上的显示效果。

   ![](assets/campaign-preview.png)

## 预览Web活动页{#preview-a-web-campaign-on-the-web-campaigns-page}上的Web活动

1. 查看Web活动列表时，只需选择一个活动并单击&#x200B;**预览**&#x200B;图标。

   ![](assets/web-campaigns-1-preview-hand.png)

   放轻松！

## 预览网站上的Web活动{#preview-a-web-campaign-on-your-website}

创建沙箱段和活动。

1. 转至&#x200B;**区段**。

   ![](assets/new-dropdown-segments-hand.jpg)

1. 单击&#x200B;**新建**。

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. 命名区段。

1. 在“行为”下，将“包括页面”拖动到画布上。 添加值*sandbox=1*。 单击&#x200B;**保存并定义活动**。

   ![](assets/segment.png)

1. 在“设置Web活动”页上，从目标中选择沙箱段，将其更改为沙箱段。

   ![](assets/set-web-campaign-target-segment.jpg)

1. 完成活动创作，然后单击&#x200B;**启动**。

   ![](assets/click-launch.jpg)

1. 转到您的网站，在URL末尾添加URL参数“？sandbox=1”。 示例：`www.marketo.com?sandbox=1`。

1. 查看活动在您的网站上的反应。

>[!NOTE]
>
>活动在访客会话期间只做一次响应。 要再次查看活动，请清除您的浏览器Cookie。

>[!NOTE]
>
>无法预览重定向活动。 测试它们的唯一方法是使用沙箱段(按特定页面进行目标- *sandbox=redirect*)
