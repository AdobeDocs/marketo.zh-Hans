---
unique-page-id: 4720145
description: 使用Google Tag Manager实施RTP - Marketo文档 — 产品文档
title: 使用Google Tag Manager实施RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用[!DNL Google Tag Manager]实施RTP {#implementing-rtp-using-google-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的[!DNL Google Tag Manager]帐户。

1. 添加新&#x200B;**[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag]。**&#x200B;调用它&#x200B;**RTP**。

1. 登录到您的&#x200B;**RTP帐户**。

1. 转到&#x200B;**[!UICONTROL Account Settings]**。

   a.如果您已从支持部门收到JavaScript标记，请继续执行步骤6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 复制RTP JavaScript标记并将其粘贴到您创建的新&#x200B;**自定义HTML标记**（步骤1）。

1. 单击&#x200B;**[!UICONTROL Add Rule to Fire Tag]**。 选择 **[!UICONTROL All Pages]**。

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;并[发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 确认它出现在所有页面上，包括登陆页面和子域。

   a.可通过右键单击网站页面来执行此操作。 转到&#x200B;**[!UICONTROL Inspect Element]**，搜索&#x200B;**RTP**&#x200B;以查找标记。
