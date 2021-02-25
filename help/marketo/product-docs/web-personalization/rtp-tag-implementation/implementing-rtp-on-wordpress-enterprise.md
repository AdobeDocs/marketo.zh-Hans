---
unique-page-id: 4720215
description: 在Wordpress Enterprise上实施RTP - Marketo Docs — 产品文档
title: 在Wordpress Enterprise上实现RTP
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# 在Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}上实现RTP

要实施RTP标签，请按照以下安装说明操作：

1. 转到&#x200B;**帐户设置**。

   a.如果您已从“支持”收到JavaScript标记 — 请继续步骤3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在“Domain（域）”下，找到相关域，然后单击“Generate Tag **（生成标记**）”。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 复制RTP JavaScript标签。

1. 以管理员用户身份登录到您的WordPress帐户

   a.在“**外观**”下，转至“**自定义JavaScript**”。
b.将RTP Javascript标签粘贴到现有代码之后。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >在粘贴代码EXCLUDE时，请执行以下标记：
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >仅插入脚本本身。

1. 单击&#x200B;**更新**。
