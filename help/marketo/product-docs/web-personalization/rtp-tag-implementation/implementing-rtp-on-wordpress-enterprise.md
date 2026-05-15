---
unique-page-id: 4720215
description: 了解如何在Marketo Engage中的wordpress enterprise中实施rtp，包括在wordpress中实施rtp。 使用本指南完成您的下一步。
title: 在 WordPress Enterprise 上实施 RTP
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 109
ht-degree: 11%

---

# 在 WordPress Enterprise 上实施 RTP {#implementing-rtp-on-wordpress-enterprise}

要实施[!UICONTROL RTP tag]，请按照以下安装说明操作：

1. 前往 **[!UICONTROL Account Settings]**。

   答： 如果您已从支持部门收到JavaScript标记 — 请继续执行步骤3。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. 复制RTP JavaScript标记。

1. 以管理员用户身份登录到您的[!DNL WordPress]帐户

   答： 在&#x200B;**[!UICONTROL Appearance]**&#x200B;下，转到&#x200B;**[!UICONTROL Custom JavaScript]**。
b. 将RTP Javascript标记粘贴到现有代码之后。

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

1. 单击 **[!UICONTROL Update]**。
