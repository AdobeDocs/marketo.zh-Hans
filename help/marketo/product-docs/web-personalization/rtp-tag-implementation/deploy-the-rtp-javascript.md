---
unique-page-id: 4719332
description: 部署RTP JavaScript - Marketo Docs —— 产品文档
title: 部署RTP JavaScript
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# 部署RTP JavaScript {#deploy-the-rtp-javascript}

要生成和设置RTP标签，请按照下面的安装说明操作

## 生成标记 {#generate-tag}

1. 登录RTP帐户。 转到“帐 **户设置**”。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 在“ **域** ”和“ **域配置**”中，找到相关域，然后单击“ **生成标记”。**

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 将Web个性化(RTP)标签复制并粘贴到您的网站中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >复制RTP JavaScript标签并将其粘贴为页面标题中的第一个脚本——在标签之 `<head> </head>` 间。

   确保标记显示在所有页面上，包括登陆页和子域。 右键单击网站页面可选中此选项。 在Web浏览器中转到视图页面源。 搜索：“RTP”。

1. 标记切换设置 **为ON**。

   确认标记切换设置为ON。 您应该开始看到数据流进组织的选项卡。

   您现在已使用RTP标签进行设置，可以 [开始创建](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) 段和实时活动!

1. 验证标记是否在所有页面上。

>[!MORELIKETHIS]
>
>* [RTP标签实现](http://docs.marketo.com/display/docs/rtp+tag+implementation)

