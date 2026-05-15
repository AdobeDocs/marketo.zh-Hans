---
unique-page-id: 11385053
description: 了解如何为预测内容生成并放置RTP Web Personalization标记。 将其复制到页头，验证覆盖范围，并确认切换是否保持打开状态。
title: 部署 Content-AI 的 JavaScript
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
TQID: https://experienceleague.adobe.com/LHzl0KuIoJvZ99eFWGFE6RdDW1xRxBS4LG3XU9ujj4U
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
source-wordcount: 152
ht-degree: 9%

---

# 部署 Content-AI 的 JavaScript {#deploy-the-javascript-for-content-ai}

要使用预测内容，您需要生成和设置RTP (Web Personalization)标记。

## 生成标记 {#generate-tag}

1. 登录您的Predictive Content帐户。 前往 **[!UICONTROL Account Settings]**。

   ![](assets/settings-dropdown-account-hands.png)

1. 在&#x200B;**[!UICONTROL Domain Configuration]**&#x200B;中，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/generate-tag.png)

1. 将Web Personalization标记复制并粘贴到网站的HTML中。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >复制Web Personalization JavaScript标记，并将其作为第一个脚本粘贴到页眉的`<head> </head>`标记之间。 请在此处查看更详细的[实施说明](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

1. 验证标记是否出现在所有页面上，包括登陆页面和子域。 可通过右键单击您网站的页面来检查此项。 在Web浏览器中转到&#x200B;**[!UICONTROL View Page Source]**。 搜索：“RTP”。

1. 确认标记切换设置为&#x200B;**[!UICONTROL ON]**。
