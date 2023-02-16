---
unique-page-id: 2360217
description: 更改Analytics的归因设置 — Marketo文档 — 产品文档
title: 更改Analytics的归因设置
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# 更改Analytics的归因设置 {#change-attribution-settings-for-analytics}

您可以更改Marketo将联系人与首次联系和多次联系归因的业务机会、潜在客户转化量度以及受营销影响的业务机会标记的联系方式。

这些设置将影响 [计划机会分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [机会分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)和潜在客户分析区域。 这也会影响程序分析器报告。

1. 转到 **管理员** 的上界。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 单击 **收入周期分析**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 单击 **编辑** 链接下 **归因**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >更改此设置不会修改任何Marketo数据；它只会更改报表的运行方式。 这可以随时恢复。

1. 选择一个选项并单击 **保存**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**条件**
   >
   >**显式**:仅具有角色的联系人（默认）。
   >
   >**混合**:具有角色的联系人（如果可用）。 如果没有可用，则会使用帐户中的所有联系人。
   >
   >**隐式**:所有联系人，不管角色如何。

>[!CAUTION]
>
>使用 **隐式**,Marketo将始终检查与该帐户关联的所有联系人，而不考虑其角色。 **Marketo强烈建议使用显式模式**. 使用隐式可能会产生误报；即，对机会有信誉的人，尽管对机会没有实际影响。 谨慎使用隐式。
