---
description: 设置MSI视图 — Marketo文档 — 产品文档
title: 设置MSI视图
hide: true
hidefromtoc: true
source-git-commit: f4930d1747f1ca893d7494afc3dcbeb8c6398e93
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 设置MSI视图 {#setting-up-msi-views}

在Dynamics中安装Sales Insight插件会自动在站点地图上添加“最佳选择”和相关功能板。 如果由于某些原因未添加功能板，请参阅下面的手动添加功能板的方法。

1. 在Dynamics中，单击齿轮图标，然后选择 **高级设置** 从下拉菜单中。

1. 在屏幕左上角，单击 **设置**. 在“自定义”下，选择“自定义”。

1. 单击 **自定义系统**.

1. 在左侧的树中，单击 **客户端扩展** 并双击 **网站地图**.

1. 单击向右箭头以转到下一页。 在“销售”下，您应会看到Marketo。 如果没有，请确保正确导入了包。

   >[!NOTE]
   >
   >在Marketo下，您应该：最佳选择、我的电子邮件、Web活动和匿名Web活动。 如果这些功能板中缺少任何功能板，请单击“销售”上方的“+”号，并将其添加为子区域。

1. 单击功能板以将其选中。 在右侧的列中，为每个列输入相应的信息。 您可以忽略未列出的任何类别。

   **最佳下注**</br>
URL:MainviewBestbets.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID:marketo_bestbets</br>
标题：最佳下注

   **我的电子邮件**</br>
URL:mkt_/MainViewMyEmail.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID:marketo_myemail</br>
标题：我的电子邮件

   **Web活动**</br>
URL:mkt_/MainViewWebActivity.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID:marketo_webactivity</br>
标题：Web活动

   **匿名Web活动**</br>
URL:mkt_/MainViewWebActivity.html</br>
图标：/WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID:marketo_anonymous_webactivity</br>
标题：匿名Web活动

1. 单击 **保存** 完成时。
