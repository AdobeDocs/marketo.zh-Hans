---
unique-page-id: 4720149
description: 在Wordpress上实施RTP - Marketo文档 — 产品文档
title: 在Wordpress上实施RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 在[!DNL Wordpress]上实施RTP {#implementing-rtp-on-wordpress}

要实施[!UICONTROL RTP tag]，请按照以下安装说明操作：

1. 打开&#x200B;**主题**&#x200B;的&#x200B;**[!DNL WordPress]header.php**&#x200B;文件。

   您可以使用FTP客户端访问服务器，或直接从[!DNL WordPress]仪表板编辑主题文件。 您的文件编辑器位于侧栏菜单的&#x200B;**[!UICONTROL Appearance]**&#x200B;选项卡下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文本编辑器右侧的模板文件列表中，找到&#x200B;**header.php**&#x200B;并将其打开。

1. 转到&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已从支持部门收到JavaScript标记 — 请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 复制RTP JavaScript标记并将其粘贴到您的网站模板中。

   a.确保它是页面标题中的第一个脚本 — **`<head> </head>`**&#x200B;标记之间。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 单击&#x200B;**[!UICONTROL Update File]**&#x200B;以获取header.php文件。

1. 验证它是否显示在包括登陆页面和子域在内的所有页面上。

   a.您可以在网站的页面上单击鼠标右键，从而执行此操作。 转到&#x200B;**[!UICONTROL View Page Source]。**&#x200B;搜索&#x200B;**RTP**&#x200B;以查找标记。
