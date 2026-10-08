---
unique-page-id: 10095389
description: 了解如何在Microsoft Dynamics中从Marketo创建联系人。 在实时创建联系人的触发营销活动中使用将人员同步到Microsoft流程操作。
title: 在 Microsoft Dynamics 中创建联系人
exl-id: 66cb26c0-f383-4d1e-be22-e7f8c6b266fb
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/5q84B57P88MNhaYHluCKKCYLwOonW2xj7hAUNDOmXl8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 5%
---
# 在[!DNL Microsoft Dynamics]中创建联系人 {#create-a-contact-in-microsoft-dynamics}

1. 选择要在Dynamics中创建为联系人的仅限Marketo Engage的人员（Microsoft类型为空）。

   ![](assets/one.png)

1. 单击&#x200B;**[!UICONTROL Person Actions]**&#x200B;和&#x200B;**[!DNL Microsoft]**，然后选择&#x200B;**[!UICONTROL Sync Person to Microsoft]**。

   ![](assets/two.png)

1. 单击&#x200B;**[!UICONTROL Sync As]**&#x200B;并选择&#x200B;**[!UICONTROL Contact]**。 单击 **[!UICONTROL Run Now]**。

   ![](assets/three.png)

   >[!NOTE]
   >
   >使用“[!UICONTROL Sync Person to Microsoft]”流程操作（仅在触发器营销活动中）时，将在Dynamics中实时创建潜在客户/联系人。

1. Marketo将[!DNL Dynamics]中的潜在客户记录限定为与[!DNL Dynamics]中的任何帐户无关联的联系人。

   ![](assets/image2015-10-23-9-3a43-3a33.png)

1. 现在，当您在智能营销活动过滤器中使用同步为约束时，可以选择&#x200B;**[!UICONTROL Contact]**。

   ![](assets/five.png)
