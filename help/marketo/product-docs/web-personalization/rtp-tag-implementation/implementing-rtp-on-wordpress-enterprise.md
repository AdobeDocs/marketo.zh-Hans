---
unique-page-id: 4720215
description: 在Wordpress Enterprise上实施RTP - Marketo文档 — 产品文档
title: 在Wordpress Enterprise上实施RTP
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# 在Wordpress Enterprise上实施RTP {#implementing-rtp-on-wordpress-enterprise}

要实施RTP标记，请按照以下安装说明操作：

1. 转到 **帐户设置**.

   a.如果您已从支持部门收到JavaScript标记，请继续执行步骤3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在“域”下，找到相关域并单击 **生成标记**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 复制RTP JavaScript标记。

1. 以管理员用户身份登录到您的WordPress帐户

   a.下 **外观**，转到 **自定义JavaScript**.
b.将RTP Javascript标记粘贴到现有代码的后面。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >粘贴代码时，请排除以下标记：
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >仅插入脚本本身。

1. 单击 **更新**.
