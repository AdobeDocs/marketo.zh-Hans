---
unique-page-id: 4720215
description: 在Wordpress Enterprise上实施RTP - Marketo Docs —— 产品文档
title: 在WordPress Enterprise上实现RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# 在WordPress Enterprise上实现RTP {#implementing-rtp-on-wordpress-enterprise}

要实施RTP标签，请按照以下安装说明操作：

1. 转到**帐户设置。**

   1. 如果您已从支持部门收到JavaScript标记，请继续执行步骤3。\
      ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在“域”下，找到相关域，然后单击“ **生成标记**”。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 复制RTP JavaScript标签。
1. 以管理员用户身份登录到您的WordPress帐户

   1. 在“ **外观**”下，转 **到“自定义JavaScript**”。
   1. 将RTP Javascript标签粘贴到现有代码之后。

      ![](assets/image2014-12-3-17-3a51-3a46.png)
   >[!CAUTION]
   >
   >粘贴代码EXCLUDE时，请执行以下标记：
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >    
   >仅插入脚本本身。

1. 单击 **更新**。
