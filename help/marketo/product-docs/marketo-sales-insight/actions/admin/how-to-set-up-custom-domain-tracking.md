---
description: 如何设置自定义域跟踪 — Marketo文档 — 产品文档
title: 如何设置自定义域跟踪
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 如何设置自定义域跟踪 {#how-to-set-up-custom-domain-tracking}

自定义域跟踪允许您的团队在添加到销售电子邮件的所有可跟踪链接中使用您自己的公司名称。 设置完此设置后，我允许列表们会您电子邮件中的任何链接，显示为go.yourcompany.com，这样当某人浏览某个链接时，该链接将读为go.yourcompany.com，而不是go.toutapp.com。

您需要IT团队的帮助，为指向go.toutapp.com的域设置CNAME记录。 此CNAME将显示在您的所有跟踪链接（例如go.yourcompany.com）上。

向IT团队确认CNAME配置正确后，即可将其添加到“操作”中的“自定义域跟踪”页面。

>[!NOTE]
>
>如果您的CNAME设置不正确，并且您在Actions中将其作为自定义域激活，则它可能会损坏跟踪链接和像素。

## 启用自定义域跟踪 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**需要管理员权限。**

1. 单击齿轮图标，然后选择 **设置**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 在“管理员设置”下，选择 **跟踪**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 在自定义域跟踪选项卡中，输入您的CNAME并单击 **连接**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
