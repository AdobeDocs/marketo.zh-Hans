---
unique-page-id: 4720149
description: 在Wordpress上实施RTP - Marketo文档 — 产品文档
title: 在Wordpress上实施RTP
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# 在Wordpress上实施RTP {#implementing-rtp-on-wordpress}

要实施RTP标记，请按照以下安装说明操作：

1. 打开 **header.php** 您的文件 **WordPress主题**.

   您可以使用FTP客户端访问服务器，或直接从WordPress仪表板编辑主题文件。 您的文件编辑器位于 **外观** 选项卡。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. 在文本编辑器右侧的模板文件列表中，查找 **header.php** 打开它。

1. 转到 **帐户设置**.

   a.如果您已从支持部门收到JavaScript标记 — 请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 在“域”下，找到相关域并单击 **生成标记**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. 复制RTP JavaScript标记并将其粘贴到您的网站模板中。

   a.确保这是页面标题的第一个脚本，介于 **`<head> </head>`** 标记之间。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. 单击 **更新文件** 标头.php文件。

1. 验证它是否显示在包括登陆页面和子域在内的所有页面上。

   a.您可以在网站的页面上单击鼠标右键，从而执行此操作。 转到 **查看页面源。** 搜索 **RTP** 以查找标记。
