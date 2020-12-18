---
unique-page-id: 4720145
description: 使用Google Tag Manager - Marketo Docs —— 产品文档实施RTP
title: 使用Google Tag Manager实现RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 0%

---


# 使用Google Tag Manager {#implementing-rtp-using-google-tag-manager}实现RTP

要实现RTP `tag please`，请按照以下安装说明操作。

1. 登录您的Google标签管理器帐户。

1. 添加新的标记>标记配置>自定义HTML标记**。**调用它&#x200B;**RTP**。

1. 登录RTP帐户**。**

1. 转到**帐户设置。**

   1. 如果您已从“支持”收到JavaScript标记，请继续执行步骤6。

      ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在“域”下，找到相关域，然后单击“生成标记”**。**

   ** ![](assets/image2014-11-30-15-3a20-3a17.png)

   **

1. 复制RTP JavaScript标签并将其粘贴到您创建的新&#x200B;**自定义HTML标签**（步骤1）。

1. 单击&#x200B;**+Add Rule to Fire Tag**。 选择&#x200B;**所有页面**。

1. 单击**保存**并[发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 验证它是否出现在所有`pages, including`登陆页和子域中。

   1. 可通过右键单击`website’s`页面来执行此操作。 转到**Inspect元素。 **搜索**RTP **以找到标记。

