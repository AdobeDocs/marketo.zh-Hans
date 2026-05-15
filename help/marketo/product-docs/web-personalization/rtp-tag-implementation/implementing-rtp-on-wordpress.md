---
unique-page-id: 4720149
description: 了解如何在Marketo Engage中的wordpress上实施rtp，包括在dnl wordpress上实施rtp。 使用本指南完成您的下一步。
title: 在 WordPress 上实施 RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 189
ht-degree: 3%

---

# 在[!DNL Wordpress]上实施RTP {#implementing-rtp-on-wordpress}

要实施[!UICONTROL RTP tag]，请按照以下安装说明操作：

1. 打开&#x200B;**[!DNL WordPress]主题**&#x200B;的&#x200B;**header.php**&#x200B;文件。

   您可以使用FTP客户端访问服务器，或直接从[!DNL WordPress]仪表板编辑主题文件。 您的文件编辑器位于侧栏菜单的&#x200B;**[!UICONTROL Appearance]**&#x200B;选项卡下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文本编辑器右侧的模板文件列表中，找到&#x200B;**header.php**&#x200B;并将其打开。

1. 前往 **[!UICONTROL Account Settings]**。

   答： 如果您已从支持部门收到JavaScript标记 — 请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 复制RTP JavaScript标记并将其粘贴到您的网站模板中。

   答： 确保它是页面标题处的第一个脚本 — **`<head> </head>`**&#x200B;标记之间。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 单击&#x200B;**[!UICONTROL Update File]**&#x200B;以获取header.php文件。

1. 验证它是否显示在包括登陆页面和子域在内的所有页面上。

   答： 要执行此操作，请右键单击您的网站页面。 转到&#x200B;**[!UICONTROL View Page Source].** 搜索&#x200B;**RTP**&#x200B;以查找标记。
