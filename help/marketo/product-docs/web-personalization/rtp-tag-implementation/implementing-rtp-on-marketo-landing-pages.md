---
unique-page-id: 4720151
description: 在Marketo登陆页面上实施RTP - Marketo文档 — 产品文档
title: 在Marketo登陆页面上实施RTP
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 在Marketo登陆页面上实施RTP {#implementing-rtp-on-marketo-landing-pages}

要实施[!UICONTROL RTP tag]，请按照以下安装说明操作：

1. 转到&#x200B;**[!UICONTROL Design Studio]。**&#x200B;打开要编辑的项目。 选择&#x200B;**[!UICONTROL Template Actions]**，选择&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在&#x200B;**HTML Source**&#x200B;选项卡上更改模板。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帐户中，转到&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已从支持部门收到JavaScript标记 — 请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 复制RTP JavaScript标记，并将其粘贴到&#x200B;**`<head> </head>`**&#x200B;标记之间的所有登陆页模板中。

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;和&#x200B;**[!UICONTROL Close]**&#x200B;窗口。

1. 返回&#x200B;**[!UICONTROL Design Studio]**，批准来自&#x200B;**[!UICONTROL Template Actions]**&#x200B;的登陆页面，单击&#x200B;**[!UICONTROL Approve]**。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最后，您需要&#x200B;**重新批准**&#x200B;使用该模板的任何登陆页面，模板更改才会生效。 您可以从主[!UICONTROL Landing Pages]部分一次重新批准所有请求。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 验证它是否显示在包括登陆页面和子域在内的所有页面上。

   要执行此操作，请右键单击您的网站页面。 转到&#x200B;**[!UICONTROL View Page Source]。**&#x200B;搜索&#x200B;**[!UICONTROL RTP]**&#x200B;以查找标记。
