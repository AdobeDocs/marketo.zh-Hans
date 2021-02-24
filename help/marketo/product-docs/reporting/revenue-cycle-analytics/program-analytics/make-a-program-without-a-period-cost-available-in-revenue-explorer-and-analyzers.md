---
unique-page-id: 2360389
description: 在收入浏览器和分析器 — Marketo Docs — 产品文档中提供无期间成本的项目
title: 在收入浏览器和分析器中提供无期间成本的项目
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# 在收入浏览器和分析器{#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}中提供无期间成本的项目

项目期间成本允许您为项目定义“金额”和“时间”。 这显示在收入周期浏览器和[分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md)中。

>[!NOTE]
>
>**需要管理权限**

某些项目可能需要包含在内，即使它们没有期限成本。 虽然您可以在期间成本中输入0，但我们使包含这些项目更简单。

>[!NOTE]
>
>项目分析器按期间成本存储项目成功。 如果没有可用的期间成本，则不会显示项目成功，而与项目的分析行为无关。 如果设置了分析行为，则将显示机会量度（渠道机会、赢取的收入等）的数据。

1. 在“管理员”部分下，单击&#x200B;**标记**。

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. 展开渠道，然后多次单击所选渠道。

   >[!NOTE]
   >
   >使用此渠道的所有项目（无论期间成本如何）都将可用于收入浏览器和分析器。 此更改将于次日生效。

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. 将“Analytics Behavior（分析行为）”更改为“Inclusive（包含）”，然后单击&#x200B;**保存**。

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>您是否注意到操作选项？ 这恰恰相反。 它不包括这些项目，而不考虑期间成本。

干得好！ 现在，使用修改后的项目的任何渠道都将包括在收入浏览器和分析器中，而无需期间成本。

>[!MORELIKETHIS]
>
>[在项目级别覆盖分析行为](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
