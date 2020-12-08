---
unique-page-id: 2360217
description: 更改Analytics的归因设置- Marketo Docs —— 产品文档
title: 更改Analytics的归因设置
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# 更改Analytics的归因设置 {#change-attribution-settings-for-analytics}

您可以更改营销人员将联系人与机会联系的方式，进行首次和多次联系归因、潜在客户转化指标以及受营销影响的机会标志。

这些设置将影响“项目机会”分析、 [“机会分析”](../../../product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)分析和“潜在客 [户](../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)”区域下的Revenue Explorer报表。 这也会影响项目分析器报告。

1. 在“管理 **员** ”部分下，单 **击收入周期分析**。

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. 单击“归 **因** ”下的“ **编辑”链接**。

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >更改此设置不会修改任何Marketo数据；它只会改变报表的运行方式。 可以随时恢复。

1. 选择一个选项，然后单击“ **保存**”。

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**定义**
   >
   >
   >**显式**:仅具有角色的联系人（默认）。
   >
   >
   >**混合**:具有角色的联系人（如果可用）。 如果没有可用，则它使用帐户中的所有联系人。
   >
   >
   >**隐式**:所有联系人，无论角色如何。

>[!CAUTION]
>
>使用隐 **式**&#x200B;时，Marketo将始终检查与帐户关联的所有联系人，而不管角色如何。 **Marketo强烈建议使用显式模式。** 使用隐式可能会产生误报；即，拥有机会信用的人，尽管对机会没有真正的影响。 谨慎使用隐式。

