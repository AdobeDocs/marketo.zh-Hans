---
unique-page-id: 4720151
description: 在Marketo登陆页上实施RTP - Marketo Docs — 产品文档
title: 在Marketo登陆页上实现RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# 在Marketo登陆页{#implementing-rtp-on-marketo-landing-pages}上实现RTP

要实施RTP标签，请按照以下安装说明操作：

1. 转到&#x200B;**Design Studio。** 打开要编辑的项目。选择&#x200B;**模板操作**，选择&#x200B;**编辑草稿**。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在&#x200B;**“HTML源**”选项卡上更改模板。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帐户中，转到&#x200B;**帐户设置**。

   a.如果您已从“支持”收到JavaScript标记 — 请继续步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在“Domain（域）”下，找到相关域，然后单击“Generate Tag **（生成标记**）”。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 复制RTP JavaScript标签并将其粘贴到&#x200B;**`<head> </head>`**&#x200B;标签之间的所有登陆页模板。

1. 单击&#x200B;**保存**&#x200B;和&#x200B;**关闭**&#x200B;窗口。

1. 返回至&#x200B;**Design Studio**，从&#x200B;**模板操作**&#x200B;批准登陆页，单击&#x200B;**批准**。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最后，您需要&#x200B;**重新批准**&#x200B;使用该模板的任何登陆页，以使模板更改生效。 您可以从主登陆页部分一次重新批准所有应用程序。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 验证它是否显示在所有页面上，包括登陆页和子域。

   您可以通过右键单击网站页面来执行此操作。 转到&#x200B;**视图页源。** 搜索 **** RTP以查找标记。
