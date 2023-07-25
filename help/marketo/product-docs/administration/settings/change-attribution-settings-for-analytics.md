---
unique-page-id: 2360217
description: 更改Analytics的归因设置 — Marketo文档 — 产品文档
title: 更改Analytics的属性设置
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# 更改Analytics的属性设置 {#change-attribution-settings-for-analytics}

您可以更改Marketo将联系人与首次联系和多点联系归因机会、商机转化量度以及受营销影响的商机标志联系的方式。

这些设置将影响 [!UICONTROL Revenue Explorer] 下的报告 [计划机会分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)， [机会分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)和潜在客户分析区域。 这也会影响 [!UICONTROL 程序分析器] 报告。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 单击 **[!UICONTROL 收入周期分析]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 单击 **[!UICONTROL 编辑]** 链接位于 **[!UICONTROL 归因]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >更改此设置不会修改任何Marketo数据，只会更改报表的运行方式。 可以随时还原。

1. 选择一个选项并单击 **[!UICONTROL 保存]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**条件**
   >
   >**[!UICONTROL 显式]**：仅具有角色的联系人（默认）。
   >
   >**[!UICONTROL 混合]**：角色联系人（如果有）。 如果没有可用联系人，则使用帐户中的所有联系人。
   >
   >**[!UICONTROL 隐式]**：所有联系人，不考虑角色。

>[!CAUTION]
>
>使用时 **[!UICONTROL 隐式]**，Marketo将始终检查与帐户关联的所有联系人，而不管角色如何。 **Marketo强烈建议使用 [!UICONTROL 显式] 模式**. 使用 [!UICONTROL 隐式] 可能会产生误报，即尽管对机会没有实际影响，但相信机会的人。 使用 [!UICONTROL 隐式] 小心点。
