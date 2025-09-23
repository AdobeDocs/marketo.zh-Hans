---
description: 设置MSI视图 — Marketo文档 — 产品文档
title: 设置 MSI 视图
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 3%

---

# 设置 MSI 视图 {#setting-up-msi-views}

在Dynamics中安装[!DNL Sales Insight]插件会自动在站点地图上添加[!DNL Best Bets]和相关仪表板。 如果由于某种原因未添加仪表板，请参阅以下说明如何手动添加仪表板。

1. 在Dynamics中，单击齿轮图标，然后从下拉列表中选择&#x200B;**[!UICONTROL Advanced Settings]**。

1. 在屏幕左上角，单击&#x200B;**[!UICONTROL Settings]**。 在“自定义”下，选择&#x200B;**[!UICONTROL Customizations]**。

1. 单击 **[!UICONTROL Customize the System]**。

1. 在左侧的树中，单击&#x200B;**[!UICONTROL Client Extensions]**&#x200B;并双击&#x200B;**[!UICONTROL Site Map]**。

1. 单击向右箭头转到下一页。 在Sales下，您应该会看到Marketo。 如果不能，请确保正确导入了包。

   >[!NOTE]
   >
   >在Marketo下，您应该有：Best Bets、My Email、Web Activity和Anonymous Web Activity。 如果缺少这些功能板，请单击Sales上方的+符号，并将它们添加为子区域。

1. 单击功能板将其选定。 在右侧的列中，为每个字段输入以下相应信息。 您可以忽略任何未列出的类别。

   **个最佳匹配**</br>
URL： MainviewBestbets.html</br>
图标： /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID： marketo_bestbets</br>
标题：最佳匹配

   **我的电子邮件**</br>
URL： mkt_/MainViewMyEmail.html</br>
图标： /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID： marketo_myemail</br>
标题：我的电子邮件

   **Web活动**</br>
URL： mkt_/MainViewWebActivity.html</br>
图标： /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID： marketo_webactivity</br>
标题： Web活动

   **匿名Web活动**</br>
URL： mkt_/MainViewWebActivity.html</br>
图标： /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID： marketo_anonymous_webactivity</br>
Title：匿名Web活动

1. 完成后单击&#x200B;**[!UICONTROL Save]**。
