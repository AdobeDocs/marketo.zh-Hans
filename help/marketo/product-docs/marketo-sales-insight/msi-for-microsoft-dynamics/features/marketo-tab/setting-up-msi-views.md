---
description: 设置MSI视图 — Marketo文档 — 产品文档
title: 设置MSI视图
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 设置MSI视图 {#setting-up-msi-views}

在Dynamics中安装Sales Insight插件会自动在站点地图上添加最佳匹配和相关功能板。 如果由于某种原因未添加仪表板，请参阅以下说明如何手动添加仪表板。

1. 在Dynamics中，单击齿轮图标并选择 **高级设置** 从下拉菜单中查找。

1. 在屏幕左上角，单击 **设置**. 在Customization下，选择 **自定义**.

1. 单击 **自定义系统**.

1. 在左侧的树中，单击 **客户端扩展** 并双击 **网站地图**.

1. 单击向右箭头转到下一页。 在Sales下，您应该会看到Marketo。 如果不能，请确保正确导入了包。

   >[!NOTE]
   >
   >在Marketo下，您应该有：Best Bets、My Email、Web Activity和Anonymous Web Activity。 如果缺少这些功能板，请单击Sales上方的+符号，并将它们添加为子区域。

1. 单击功能板将其选定。 在右侧的列中，为每个字段输入以下相应信息。 您可以忽略任何未列出的类别。

   **最佳匹配**</br>
URL： MainviewBestbets.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID：marketo_bestbets</br>
标题：最佳匹配

   **我的电子邮件**</br>
URL： mkt_/MainViewMyEmail.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID：marketo_myemail</br>
标题：我的电子邮件

   **Web活动**</br>
URL： mkt_/MainViewWebActivity.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID：marketo_webactivity</br>
标题： Web活动

   **匿名Web活动**</br>
URL： mkt_/MainViewWebActivity.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID：marketo_anonymous_webactivity</br>
Title：匿名Web活动

1. 单击 **保存** 完成时。
