---
unique-page-id: 4720145
description: 了解如何在Marketo Engage中使用google标签管理器实施rtp，包括使用dnl google实施rtp。 使用本指南完成您的下一步。
title: 使用 Google 标记管理器实施 RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 152
ht-degree: 6%

---

# 使用[!DNL Google Tag Manager]实施RTP {#implementing-rtp-using-google-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的[!DNL Google Tag Manager]帐户。

1. 添加新&#x200B;**[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag].** 将其命名为&#x200B;**RTP**。

1. 登录到您的&#x200B;**RTP帐户**。

1. 前往 **[!UICONTROL Account Settings]**。

   答： 如果您已从支持部门收到JavaScript标记，请继续执行步骤6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 复制RTP JavaScript标记并将其粘贴到您创建的新&#x200B;**自定义HTML标记**（步骤1）。

1. 单击 **[!UICONTROL Add Rule to Fire Tag]**。 选择 **[!UICONTROL All Pages]**。

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;并[发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 确认它出现在所有页面上，包括登陆页面和子域。

   答： 要执行此操作，请右键单击您网站的页面。 转到&#x200B;**[!UICONTROL Inspect Element]**，搜索&#x200B;**RTP**&#x200B;以查找标记。
