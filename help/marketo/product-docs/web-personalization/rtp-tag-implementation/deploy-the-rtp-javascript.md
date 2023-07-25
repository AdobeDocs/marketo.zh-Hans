---
unique-page-id: 4719332
description: 部署RTP JavaScript - Marketo文档 — 产品文档
title: 部署RTP JavaScript
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# 部署RTP JavaScript {#deploy-the-rtp-javascript}

要生成和设置您的RTP标记，请按照下面的安装说明操作

## 生成标记 {#generate-tag}

1. 登录到您的RTP帐户。 转到 **帐户设置**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. In **域** 和 **域配置**，找到相关域并单击 **生成标记**.

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 将Web个性化(RTP)标记复制并粘贴到您的网站中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >复制RTP JavaScript标记并将其粘贴为页面标题中的第一个脚本 — 在 `<head> </head>` 标记之间。

   确保标记出现在所有页面上，包括登陆页面和子域。 右键单击您网站的页面以检查此项。 转到Web浏览器中的查看页面源。 搜索：“RTP”。

1. 标记切换设置为 **日期**.

   确认标记切换开关已设置为开。 您应该会开始看到数据流入组织的选项卡。

   您现在已设置RTP标记并准备开始 [创建区段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) 和实时营销活动！

1. 验证标记是否位于所有页面上。
