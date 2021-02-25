---
unique-page-id: 4720149
description: 在Wordpress上实施RTP - Marketo Docs — 产品文档
title: 在Wordpress上实现RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---


# 在Wordpress {#implementing-rtp-on-wordpress}上实现RTP

要实施RTP标签，请按照以下安装说明操作：

1. 打开&#x200B;**WordPress主题**&#x200B;的&#x200B;**header.php**&#x200B;文件。

   您可以使用FTP客户端访问服务器或直接从WordPress仪表板编辑主题文件。 您的文件编辑器位于侧栏菜单的&#x200B;**外观**&#x200B;选项卡下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文本编辑器右侧的模板文件列表中，找到&#x200B;**header.php**&#x200B;并打开它。

1. 转到&#x200B;**帐户设置**。

   a.如果您已从“支持”收到JavaScript标记 — 请继续步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在“Domain（域）”下，找到相关域，然后单击“Generate Tag **（生成标记**）”。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 复制RTP JavaScript标签并将其粘贴到您的网站模板。

   a.确保它是页面标题中位于&#x200B;**`<head> </head>`**&#x200B;标记之间的第一个脚本。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 单击&#x200B;**更新文件**&#x200B;获取header.php文件。

1. 验证它是否显示在所有页面上，包括登陆页和子域。

   a.您可以通过右键单击网站页面来执行此操作。 转到&#x200B;**视图页源。** 搜索 **** RTP以查找标记。
