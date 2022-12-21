---
unique-page-id: 2360421
description: 覆盖项目级别的Analytics行为 — Marketo文档 — 产品文档
title: 在项目级别覆盖分析行为
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 在项目级别覆盖分析行为 {#override-analytics-behavior-at-the-program-level}

您可以设置 [管理员级别对渠道的分析行为](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md) 但您也可以在程序级别覆盖它。 以下是操作方法：

1. 转到 **营销活动** 的上界。

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. 查找并选择您的项目。

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. 在 **设置** ，请将Analytics行为拖到画布中。

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. 选择所需的Analytics行为。

   >[!NOTE]
   >
   >**条件**
   >
   >* **包含**  — 此选项将确保该程序可用于在收入浏览器和分析程序中报告，而无论您是否包含期间成本。
   >* **运行**  — 此选项会导致项目在收入浏览器或分析程序中均不显示。


   >[!NOTE]
   >
   >默认行为（如果未应用此设置）是程序将包含在Analytics中 **仅当至少有一个期间成本时**，即使分配了零美元。

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. 单击 **保存**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

干得好！ 现在，您了解如何覆盖项目级别的分析行为。

>[!NOTE]
>
>这些更改将在次日生效，并且将可用或从收入浏览器和分析程序中取出。
