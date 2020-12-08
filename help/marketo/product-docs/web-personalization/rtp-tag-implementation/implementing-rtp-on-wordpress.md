---
unique-page-id: 4720149
description: 在Wordpress上实施RTP - Marketo Docs —— 产品文档
title: 在Wordpress上实现RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# 在Wordpress上实现RTP {#implementing-rtp-on-wordpress}

要实施RTP标签，请按照以下安装说明操作：

1. 打开WordPress **主题的header** .php **文件**。

   您可以使用FTP客户端访问服务器或直接从WordPress仪表板编辑主题文件。 文件编辑器位于提要栏菜单 **的** “外观”选项卡下。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文本编辑器右侧的模板文件列表中，找 **到header.php** ，然后打开它。
1. 转到“帐 **户设置”。**

   如果您已从支持部门收到JavaScript标记，请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在“域”下，找到相关域，然后单击“ **生成标记**”。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 复制RTP JavaScript标签并将其粘贴到您的网站模板。

   确保它是页面标题中位于标记之间的第一个脚 **`<head> </head>`** 本。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 单击 **头。php文** 件的“更新文件”。
1. 验证它是否出现在所 `pages including` 有登陆页和子域上。

   您可以通过右键单击页面来执行此 `website’s` 操作。 转到 **视图页面源。** 搜索 **RTP** 以找到标记。
