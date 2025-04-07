---
description: 将SSL添加到登陆页面 — Marketo文档 — 产品文档
title: 将SSL添加到登陆页面
hide: true
hidefromtoc: true
feature: Landing Pages
source-git-commit: f41d0595db695fc485a209aa2f9646a76e57acdf
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 将SSL添加到登陆页面 {#add-ssl-to-your-landing-pages}

了解如何将品牌域的别名（例如，`http://business.adobe.com`）添加到Marketo Engage中创建的登陆页面，以便能够在其品牌域下访问这些页面。

屏幕快照

## 启用SSL认证 {#enable-ssl-certification}

自动为您在登陆页面规则中创建的所有域别名添加SSL。

1. 转到&#x200B;**管理员**&#x200B;区域。

   屏幕快照

1. 从树中选择&#x200B;**登陆页面**。 在&#x200B;**规则**&#x200B;选项卡中，单击&#x200B;**新建**&#x200B;下拉列表，然后选择&#x200B;**新建域别名**。

   屏幕快照

1. 选中&#x200B;**生成SSL证书**&#x200B;复选框。

   屏幕快照

这会自动为此域添加SSL证书。

屏幕快照

## 为默认域启用SSL

屏幕快照

注释：

列表中的“SSL证书”列将显示在此功能发布后创建的所有域别名的SSL证书状态。 如果您通过支持为域启用了SSL，则相应的SSL证书将继续存在，但此表仅反映使用此功能添加的域的SSL证书

SSL处于“就绪”状态最多可能需要3分钟，并且用户需要刷新页面才能将更改传播到UI上。
