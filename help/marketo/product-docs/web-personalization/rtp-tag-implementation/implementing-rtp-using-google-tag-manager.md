---
unique-page-id: 4720145
description: 使用Google Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用Google Tag Manager实施RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# 使用Google Tag Manager实施RTP {#implementing-rtp-using-google-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的Google Tag Manager帐户。

1. 添加新标记>标记配置>自定义HTML标记**。**将其命名为&#x200B;**RTP**。

1. 登录到您的RTP帐户**。**

1. 转到&#x200B;**帐户设置**。

   a.如果您已从支持部门收到JavaScript标记，请继续执行步骤6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在“域”下，找到相关域，然后单击&#x200B;**生成标记**。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 复制RTP JavaScript标签并将其粘贴到您创建的新&#x200B;**自定义HTML标签**（步骤1）。

1. 单击&#x200B;**+添加规则以触发标记**。 选择&#x200B;**所有页面**。

1. 单击&#x200B;**保存**&#x200B;和[发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 确认它出现在所有页面上，包括登陆页面和子域。

   a.可通过右键单击网站页面来执行此操作。 转到&#x200B;**Inspect元素**，搜索&#x200B;**RTP**&#x200B;以查找标记。
