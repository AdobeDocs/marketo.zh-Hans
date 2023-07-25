---
description: 如何设置自定义域跟踪 — Marketo文档 — 产品文档
title: 如何设置自定义域跟踪
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 如何设置自定义域跟踪 {#how-to-set-up-custom-domain-tracking}

自定义域跟踪允许您的团队在添加到您的销售电子邮件中的所有可跟踪链接中使用您自己的公司名称。 完成此设置后，我们将允许列表您在电子邮件中的任何链接，使其显示为go.yourcompany.com，这样当有人将鼠标悬停在链接上时，它将会显示go.yourcompany.com而不是go.toutapp.com。

您需要IT团队的帮助，才能为指向go.toutapp.com的域设置CNAME记录。 此CNAME将成为您所有跟踪链接(例如go.yourcompany.com)上显示的内容。

向IT团队确认已正确配置CNAME后，您可以将其添加到“操作”中的“自定义域跟踪”页面。

>[!NOTE]
>
>如果未正确设置CNAME，并且您在“操作”中将其激活为自定义域，则它可能会破坏跟踪链接和像素。

## 启用自定义域跟踪 {#enable-custom-domain-tracking}

>[!NOTE]
>
>**需要管理员权限。**

1. 单击齿轮图标并选择 **设置**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. 在管理设置下，选择 **跟踪**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. 在自定义域跟踪选项卡中，输入您的CNAME并单击 **Connect**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
