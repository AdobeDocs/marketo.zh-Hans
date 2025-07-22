---
description: 如何设置自定义域跟踪 — Marketo文档 — 产品文档
title: 如何设置自定义域跟踪
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# 如何设置自定义域跟踪 {#how-to-set-up-custom-domain-tracking}

自定义域跟踪允许您的团队在添加到销售电子邮件的所有可跟踪链接中使用您自己的公司名称。 完成此设置后，我们将允许列表您在电子邮件中的任何链接，使其显示为go.yourcompany.com，这样当有人将鼠标悬停在链接上时，它将会显示go.yourcompany.com而不是go.toutapp.com。

您需要获得IT团队的帮助，才能为指向go.toutapp.com的域设置CNAME记录。 此CNAME将显示在所有跟踪链接上(例如go.yourcompany.com)。

向IT团队确认已正确配置CNAME后，您可以将其添加到“操作”中的[!UICONTROL Custom Domain Tracking]页面。

>[!NOTE]
>
>如果未正确设置CNAME，并且您在操作中将它激活为自定义域，它可能会破坏跟踪链接和像素。

## 启用自定义域跟踪 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**需要管理员权限。**

1. 单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 在[!UICONTROL Admin Settings]下，选择&#x200B;**[!UICONTROL Tracking]**。

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 在[!UICONTROL Custom Domain Tracking]选项卡中，输入您的CNAME并单击&#x200B;**[!UICONTROL Connect]**。

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
