---
unique-page-id: 2360389
description: 在“收入浏览器”和“分析器 — Marketo文档 — 产品文档”中提供不含期间成本的计划
title: 在收入浏览器和分析程序中，使没有期间成本的程序可用
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 在收入浏览器和分析程序中，使没有期间成本的程序可用 {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

计划期间成本允许您为计划定义“金额”和“时间”。 此参数显示在收入周期浏览器和 [分析程序](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**需要管理员权限**

有些项目即使没有周期成本，也可能需要包含在内。 虽然您可以在期间成本中输入0，但我们已更轻松地包含这些程序。

>[!NOTE]
>
>程序分析器按期间成本存储程序成功。 如果没有可用的时段成本，则无论项目的分析行为如何，都不会显示项目成功。 如果设置了分析行为，则将显示机会量度（管道商机、赢得的收入等）的数据。

1. 在管理员部分下，单击 **标记**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. 展开渠道，然后双击所选渠道。

   >[!NOTE]
   >
   >使用此渠道的所有项目（不论期间成本如何）都将可用于收入浏览器和分析程序。 此更改将于次日生效。

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. 将Analytics行为更改为“包含”，然后单击 **保存**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>您是否注意到操作选项？ 这恰恰相反。 它不包括这些方案，而不考虑期间费用。

干得好！ 现在，使用修改后渠道的任何程序都将包含在收入浏览器和分析程序中，而无需支付期间成本。

>[!MORELIKETHIS]
>
>[在项目级别覆盖分析行为](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
