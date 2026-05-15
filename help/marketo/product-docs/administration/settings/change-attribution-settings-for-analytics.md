---
unique-page-id: 2360217
description: 如何在Revenue Cycle Analytics中设置首次联系和多联系归因、商机转化和受营销影响的机会选项。
title: 更改分析的归因设置
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 160
ht-degree: 9%

---

# 更改分析的归因设置 {#change-attribution-settings-for-analytics}

您可以更改Marketo将联系人与首次联系和多次联系归因机会、商机转化量度以及受营销影响的商机标志关联的方式。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 单击 **[!UICONTROL Revenue Cycle Analytics]**。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 单击&#x200B;**[!UICONTROL Attribution]**&#x200B;下的&#x200B;**[!UICONTROL Edit]**&#x200B;链接。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >更改此设置不会修改任何Marketo数据，而是会更改报表的运行方式。 可以随时撤消此操作。

1. 选择一个选项，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定义**
   >
   >**[!UICONTROL Explicit]**：仅具有角色的联系人（默认）。
   >
   >**[!UICONTROL Hybrid]**：具有角色的联系人（如果可用）。 如果没有可用联系人，则它会使用帐户中的所有联系人。
   >
   >**[!UICONTROL Implicit]**：所有联系人，不考虑角色。

>[!CAUTION]
>
>使用&#x200B;**[!UICONTROL Implicit]**&#x200B;时，Marketo将始终检查与该帐户关联的所有联系人，不论角色如何。 **Marketo强烈建议使用[!UICONTROL Explicit]模式**。 使用[!UICONTROL Implicit]可能会产生误报；即，尽管对机会没有实际影响，但拥有机会信用的人员。 请谨慎使用[!UICONTROL Implicit]。
