---
unique-page-id: 4720151
description: 在Marketo登陆页面上实施RTP - Marketo文档 — 产品文档
title: 在Marketo登陆页面上实施RTP
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# 在Marketo登陆页面上实施RTP {#implementing-rtp-on-marketo-landing-pages}

要实施RTP标记，请按照以下安装说明操作：

1. 转到 **Design Studio。** 打开要编辑的项目。 选择 **模板操作**，选择 **编辑草稿**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在上更改模板 **HTML源** 选项卡。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在您的RTP帐户中，转到 **帐户设置**.

   a.如果您已从支持部门收到JavaScript标记 — 请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在“域”下，找到相关域并单击 **生成标记**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 复制RTP JavaScript标记并将其粘贴到您的所有登陆页面模板中的 **`<head> </head>`** 标记之间。

1. 单击 **保存** 和 **关闭** 窗户。

1. 返回 **Design Studio**，审批登陆页面 **模板操作**，单击 **批准**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最后，您需要 **重新批准** 使用该模板的任何登陆页面都将进行更改以生效。 您可以一次从主登陆页面部分重新批准所有这些请求。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 验证它是否显示在包括登陆页面和子域在内的所有页面上。

   要执行此操作，请右键单击您的网站页面。 转到 **查看页面源。** 搜索 **RTP** 以查找标记。
