---
unique-page-id: 4720145
description: 使用Google标签管理器实施RTP - Marketo文档 — 产品文档
title: 使用Google标签管理器实施RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# 使用Google标签管理器实施RTP {#implementing-rtp-using-google-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的Google Tag Manager帐户。

1. 添加新的标记>标记配置>自定义HTML标记**。**叫它 **RTP**.

1. 登录到您的RTP帐户**。**

1. 转到 **帐户设置**.

   a.如果您已从“支持”中收到JavaScript标记，请继续执行步骤6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在“域”下，找到相关域并单击 **生成标记**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 复制RTP JavaScript标记并将其粘贴到新 **自定义HTML标记** 已创建（步骤1）。

1. 单击 **+将规则添加到触发标记**. 选择 **所有页面**.

1. 单击 **保存** 和 [发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. 验证该页面是否显示在所有页面上，包括登陆页面和子域。

   a.您可以通过右键单击您网站的页面来执行此操作。 转到 **Inspect元素**，搜索 **RTP** 来查找标记。
