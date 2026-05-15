---
unique-page-id: 4719332
description: 了解如何在Marketo Engage中部署rtp javascript，包括部署rtp javascript。 使用本指南完成您的下一步。
title: 部署 RTP JavaScript
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XUylNa8clUib-aMhpAR8fjeu4pHRA8KSQydSH1AVxF8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 171
ht-degree: 5%

---

# 部署 RTP JavaScript {#deploy-the-rtp-javascript}

要生成和设置您的RTP标记，请按照下面的安装说明操作

## [!UICONTROL Generate Tag] {#generate-tag}

1. 登录到您的RTP帐户。 前往 **[!UICONTROL Account Settings]**。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 在&#x200B;**[!UICONTROL Domain]**&#x200B;和&#x200B;**[!UICONTROL Domain Configuration]**&#x200B;中，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 将Web Personalization (RTP)标记复制并粘贴到您的网站中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >复制RTP JavaScript标记，并将其粘贴为页眉中的第一个脚本 — 在`<head> </head>`标记之间。

   确保标记出现在所有页面上，包括登陆页面和子域。 可通过右键单击您网站的页面来检查此项。 在Web浏览器中转到查看页面Source 。 搜索：“RTP”。

1. [!UICONTROL Tag]切换设置为&#x200B;**[!UICONTROL ON]**。

   确认[!UICONTROL Tag]切换设置为[!UICONTROL ON]。 您应该会看到数据开始流入组织的选项卡。

   您现在已经设置了RTP标记，可以开始[创建区段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)和实时营销活动！

1. 验证标记是否位于所有页面上。
