---
unique-page-id: 2360421
description: 覆盖项目级别的Analytics行为 — Marketo文档 — 产品文档
title: 覆盖项目级别的Analytics行为
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 覆盖项目级别的Analytics行为 {#override-analytics-behavior-at-the-program-level}

您可以设置 [对渠道的管理员级别的Analytics行为](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md) 但您也可以在项目级别覆盖它。 方法如下：

1. 转到 **营销活动** 区域。

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. 查找并选择您的项目。

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. 在 **设置** 选项卡，将Analytics行为拖到画布中。

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. 选择所需的Analytics行为。

   >[!NOTE]
   >
   >**条件**
   >
   >* **包含**  — 此选项将确保程序可用于在收入资源管理器和分析器中报告，无论您是否包括期间成本。
   >* **可操作**  — 此选项导致该程序不会显示在收入资源管理器或分析器中。

   >[!NOTE]
   >
   >默认行为（如果未应用此设置）是Analytics中将包含程序 **仅当至少有一个期间成本时**，即使分配了零美元也是如此。

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. 单击 **保存**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

做得好！ 现在您知道如何在程序级别覆盖分析行为了。

>[!NOTE]
>
>这些更改将在第二天生效，并且或者可供使用，或者从收入资源管理器和分析器中提取。
