---
unique-page-id: 10092925
description: 预览和测试Web营销活动 — Marketo文档 — 产品文档
title: 预览并测试 Web 营销活动
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 4%

---

# 预览并测试 Web 营销活动 {#preview-and-test-a-web-campaign}

本文向您说明预览Web营销活动的不同方式，以及如何使用网站上实时显示的沙盒区段测试营销活动。

>[!NOTE]
>
>预览仅会显示促销活动在选定网站上的外观。 链接和小组件将无法使用，因为会避免Analytics中的错误点击/查看。

## 在创建页面上预览Web营销活动 {#preview-a-web-campaign-on-the-creation-page}

1. 转到&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. 单击&#x200B;**[!UICONTROL Create New Web Campaign]**&#x200B;或图标以编辑现有营销策划。

   ![](assets/create-new-or-edit-web-campaign.png)

1. 在网站预览中，添加页面URL并单击&#x200B;**[!UICONTROL Preview]**。 此时将打开一个新窗口/选项卡，其中显示了营销活动预览。

   ![](assets/three-1.png)

   >[!TIP]
   >
   >单击&#x200B;**[!UICONTROL Share]**&#x200B;以打开包含营销活动预览的固定URL的电子邮件。

   >[!NOTE]
   >
   >您还可以选择安装浏览器插件（[[!DNL Chrome]](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj)或[[!DNL Firefox]](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)），以获得预览促销活动的最佳体验。 请参阅以下部分。

## 使用浏览器插件在“创建”页面上预览Web营销活动 {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. 按照上节中的步骤1和2操作。

1. 单击指向浏览器插件的链接（在本例中，我们使用的是[!DNL Chrome]）。

   ![](assets/4-1.png)

1. 此时将打开一个新窗口/选项卡。 单击 **[!UICONTROL Add to Chrome]**。

   ![](assets/five.png)

1. 单击 **[!UICONTROL Add Extension]**。

   ![](assets/six.png)

1. 返回Marketo。 添加页面URL并单击&#x200B;**[!UICONTROL Preview]**。

   ![](assets/seven.png)

1. 这将打开一个新窗口/选项卡，允许您预览促销活动在桌面、手机或平板电脑上的外观。

   ![](assets/campaign-preview.png)

## 在Web营销活动页面上预览Web营销活动 {#preview-a-web-campaign-on-the-web-campaigns-page}

1. 在查看Web促销活动列表时，只需选择一个促销活动并单击&#x200B;**[!UICONTROL Preview]**&#x200B;图标即可。

   ![](assets/web-campaigns-1-preview-hand.png)

   放轻松！

## 在网站上预览Web营销活动 {#preview-a-web-campaign-on-your-website}

创建沙盒区段和营销活动。

1. 转到&#x200B;**[!UICONTROL Segments]**。

   ![](assets/new-dropdown-segments-hand.jpg)

1. 单击 **[!UICONTROL Create New]**。

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. 命名区段。

1. 在[!UICONTROL Behavioral]下，将[!UICONTROL Include Pages]拖到画布上。 添加值&#42;sandbox=1&#42;。 单击 **[!UICONTROL Save & Define Campaign]**。

   ![](assets/segment.png)

1. 在设置Web营销活动页面上，通过从列表中选择目标区段将其更改为沙盒区段。

   ![](assets/set-web-campaign-target-segment.jpg)

1. 完成活动创意并单击&#x200B;**[!UICONTROL Launch]**。

   ![](assets/click-launch.jpg)

1. 转到您的网站，在URL的末尾添加URL参数“？sandbox=1”。 示例：`www.marketo.com?sandbox=1`。

1. 请参阅您网站上的营销活动反应。

>[!NOTE]
>
>营销活动在访客会话期间只反应一次。 要再次查看营销活动，请清除您的浏览器Cookie。

>[!NOTE]
>
>无法预览重定向营销活动。 测试它们的唯一方法是使用沙盒区段（按特定页面定位 — &#42;沙盒=重定向&#42;）
