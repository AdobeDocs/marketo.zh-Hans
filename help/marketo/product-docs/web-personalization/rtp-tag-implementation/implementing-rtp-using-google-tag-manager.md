---
unique-page-id: 4720145
description: 了解如何在Marketo Engage中使用google标签管理器实施rtp，包括使用dnl google实施rtp。 使用本指南完成您的下一步。
title: 使用 Google 标记管理器实施 RTP
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 6%

---

# 使用[!DNL Google Tag Manager]实施RTP {#implementing-rtp-using-google-tag-manager}

要实施RTP标记，请按照以下安装说明操作。

1. 登录到您的[!DNL Google Tag Manager]帐户。

1. 添加新&#x200B;**[!UICONTROL Tag]** > **[!UICONTROL Tag Configurations]** > **[!UICONTROL Custom HTML Tag]。**&#x200B;调用它&#x200B;**RTP**。

1. 登录到您的&#x200B;**RTP帐户**。

1. 前往 **[!UICONTROL Account Settings]**。

   a.如果您已从支持部门收到JavaScript标记，请继续执行步骤6。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 在[!UICONTROL Domain]下，找到相关域并单击&#x200B;**[!UICONTROL Generate Tag]**。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. 复制RTP JavaScript标记并将其粘贴到您创建的新&#x200B;**自定义HTML标记**（步骤1）。

1. 单击 **[!UICONTROL Add Rule to Fire Tag]**。 选择 **[!UICONTROL All Pages]**。

1. 单击&#x200B;**[!UICONTROL Save]**&#x200B;并[发布新版本](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. 确认它出现在所有页面上，包括登陆页面和子域。

   a.可通过右键单击网站页面来执行此操作。 转到&#x200B;**[!UICONTROL Inspect Element]**，搜索&#x200B;**RTP**&#x200B;以查找标记。
