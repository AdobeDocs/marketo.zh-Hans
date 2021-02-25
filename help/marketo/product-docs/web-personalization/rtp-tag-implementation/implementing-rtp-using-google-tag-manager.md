---
unique-page-id: 4720145
description: 使用Google Tag Manager - Marketo Docs — 产品文档实施RTP
title: 使用Google标签管理器实现RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# 使用Google标签管理器{#implementing-rtp-using-google-tag-manager}实现RTP

要实施RTP标签，请按照以下安装说明操作。

1. 登录到您的Google Tag Manager帐户。

1. 添加新的“标签”>“标签配置”>“自定义HTML标签”**。**将其调用为&#x200B;**RTP**。

1. 登录RTP帐户**。**

1. 转到&#x200B;**帐户设置**。

   a.如果您已从“支持”收到JavaScript标记，请继续执行步骤6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在“Domain（域）”下，找到相关域，然后单击“Generate Tag **（生成标记**）”。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 复制RTP JavaScript标签并将其粘贴到您创建的新&#x200B;**自定义HTML标签**（步骤1）。

1. 单击&#x200B;**+添加规则以触发标记**。 选择&#x200B;**所有页面**。

1. 单击&#x200B;**保存**&#x200B;和[发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 验证它是否显示在所有页面上，包括登陆页和子域。

   a.您可以通过右键单击网站页面来执行此操作。 转到&#x200B;**Inspect元素**，搜索&#x200B;**RTP**&#x200B;以查找标记。
