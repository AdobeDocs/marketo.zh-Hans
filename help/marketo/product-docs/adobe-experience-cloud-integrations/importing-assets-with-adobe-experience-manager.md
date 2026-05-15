---
unique-page-id: 37355768
description: 了解如何将资源从Adobe Experience Manager导入Marketo Design Studio。 使用资源选择器访问、选择AEM图像，并将其引入您的Marketo营销活动。
title: 使用 Adobe Experience Manager 导入资源
exl-id: 56ccf38f-3c99-4018-9989-719854e37a20
feature: Integrations
TQID: https://experienceleague.adobe.com/DQqJuvBbIZwHVKae9T3NknMvdGG0-f5Al1ERxnaotl8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 6%

---

# 使用 Adobe Experience Manager 导入资源 {#importing-assets-with-adobe-experience-manager}

资产选择器允许Marketo客户访问、选择AEM资产，并将其导入Marketo [!DNL Design Studio]。 **需要管理员权限**。

>[!AVAILABILITY]
>
>并非每个人都购买了此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

>[!PREREQUISITES]
>
>确保已执行[AEM配置](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/configuring-adobe-experience-manager-integration.md)。

>[!IMPORTANT]
>
>当前，[!DNL Firefox]中完全支持此功能。 [!DNL Safari]不支持它，并且它可能在[!DNL Chrome]的最新版本中不起作用，具体取决于您的[!DNL SameSite] Cookie设置。

1. 单击 **[!UICONTROL Design Studio]**。

   ![](assets/importing-assets-with-adobe-experience-manager-1.png)

1. 单击“新建”下拉菜单并选择&#x200B;**[!UICONTROL Import from Adobe Experience Manager]**。

   ![](assets/importing-assets-with-adobe-experience-manager-2.png)

1. 选择图像将保存到的文件夹。

   ![](assets/importing-assets-with-adobe-experience-manager-3.png)

1. 登录到Adobe Experience Manager（如果尚未登录）。

   ![](assets/importing-assets-with-adobe-experience-manager-4.png)

1. 选择您的文件夹。 然后，通过单击缩略图选择所需的图像（最多可选择10张）。 完成后，单击 **[!UICONTROL Select]**。

   ![](assets/importing-assets-with-adobe-experience-manager-5.png)

   >[!NOTE]
   >
   >图像大小不能超过100MB。

1. 单击&#x200B;**[!UICONTROL Import]**&#x200B;以完成该过程。

   ![](assets/importing-assets-with-adobe-experience-manager-6.png)

   单击&#x200B;**[!UICONTROL Close]**&#x200B;以返回设计工作室。

   ![](assets/importing-assets-with-adobe-experience-manager-7.png)

## 注意事项 {#things-to-note}

* Marketo当前支持Adobe Experience Manager版本6.4和6.5。

* 实例中的所有用户都将能够查看和访问您导入的图像。

* 图像不会自动更新。 如果导入到Marketo [!DNL Design Studio]中的图像在AEM中更新，则必须手动将其重新导入到Marketo中。
