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


# 更改分析{#change-attribution-settings-for-analytics}的归因设置

您可以更改营销人员将联系人与机会联系的方式，进行首次和多次联系归因、潜在客户转化指标以及受营销影响的机会标志。

这些设置将影响[项目机会分析](../../../product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)、[机会分析](../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)和潜在客户分析区域下的收入浏览器报告。 这也会影响项目分析器报告。

1. 在&#x200B;**Admin**&#x200B;部分下，单击&#x200B;**收入周期分析**。

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. 单击&#x200B;**Attribution**&#x200B;下的&#x200B;**Edit**&#x200B;链接。

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >更改此设置不会修改任何Marketo数据；它只会改变报表的运行方式。 可以随时恢复。

1. 选择一个选项，然后单击&#x200B;**保存**。

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**定义**
   >
   >
   >**显式**:仅具有角色的联系人（默认）。
   >
   >
   >**混合**:具有角色的联系人（如果可用）。如果没有可用，则它使用帐户中的所有联系人。
   >
   >
   >**隐式**:所有联系人，无论角色如何。

>[!CAUTION]
>
>使用&#x200B;**Implicit**&#x200B;时，Marketo将始终检查与帐户关联的所有联系人，而不管角色如何。 **Marketo强烈建议使用显式模式。** 使用隐式可能会产生误报；即，拥有机会信用的人，尽管对机会没有真正的影响。谨慎使用隐式。

