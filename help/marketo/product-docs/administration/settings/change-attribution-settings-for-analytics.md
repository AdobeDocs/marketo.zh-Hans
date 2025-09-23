---
unique-page-id: 2360217
description: 更改Analytics的归因设置 — Marketo文档 — 产品文档
title: 更改分析的归因设置
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 8%

---

# 更改分析的归因设置 {#change-attribution-settings-for-analytics}

您可以更改Marketo将联系人与首次联系和多次联系归因机会、商机转化量度以及受营销影响的商机标志关联的方式。

这些设置将影响[!UICONTROL Revenue Explorer]计划机会分析[、](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)机会分析[和潜在客户分析区域下的](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)报告。 这也会影响[!UICONTROL Program Analyzer]报表。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 单击 **[!UICONTROL Revenue Cycle Analytics]**。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 单击&#x200B;**[!UICONTROL Edit]**&#x200B;下的&#x200B;**[!UICONTROL Attribution]**&#x200B;链接。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >更改此设置不会修改任何Marketo数据，只会更改报表的运行方式。 可以随时撤消此操作。

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
