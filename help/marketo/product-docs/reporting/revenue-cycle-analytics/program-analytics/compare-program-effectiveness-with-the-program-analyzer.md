---
unique-page-id: 2360403
description: 使用程序分析器比较程序有效性 — Marketo文档 — 产品文档
title: 使用程序分析器比较程序有效性
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 使用程序分析器比较程序有效性 {#compare-program-effectiveness-with-the-program-analyzer}

使用Program Analyzer通过比较项目成本、成员获取、渠道和收入，确定最有效和最不有效的项目。

>[!PREREQUISITES]
>
>[创建程序分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 单击 **分析**.

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 选择程序分析器。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 将“View to By Program（按程序查看）”更改为。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. 使用渠道筛选器将视图缩小到仅一个或两个渠道。 现在，我们来看一下贸易展览频道中的节目。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >将程序过滤到某个渠道的快速方法是选择 **视图** > **按渠道**，单击该渠道的泡泡，然后在弹出对话框中单击渠道名称。

1. 使用X轴下拉菜单选择水平轴的量度。 我们将从计划成本开始。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 使用Y轴下拉菜单选择垂直轴的量度。 让我们选择“新名称”来查找能够捕捉新商机的程序。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. 打开滑块以放大。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >您也可以尝试通过从线性缩放更改为对数缩放来改善视图，反之亦然。 使用 **缩放** 菜单。

1. 浏览生成的图表。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   在我们的例子中，我们了解到折纸世博会在获取新名称方面远远优于该渠道中的所有其他项目，而且成本适中。 但这不是故事的全部。 我们将再添加两个量度以加深了解。

1. 使用气泡大小下拉列表选择要按气泡大小进行比较的量度。 我们将选择(FT) Revenue Won作为示例。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >您可以在程序分析器中选择的许多量度都可用于首次联系(FT)和多点联系(MT)计算。 了解 [ft和MT归因之间的差异](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. 观看图表中的气泡变化大小。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   通过添加 **(FT)已获得的收入**，我们很快看到，虽然折纸世博会获得了许多新名字，但收入却相对较少。 此外，我们看到Paper Fest 12计划越来越少，但名字越来越好，因为它会影响赢得的更多收入（更大的泡沫）。

1. 使用颜色下拉菜单添加第四个量度。 我们将了解(FT)收入与投资。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. 观察图形中的颜色变化。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

我们看到，纸汇十二节目不仅影响更多的收入（更大的泡沫），而且尽管它的节目成本相对较高（位于最右边），但在贸易展览频道的所有节目中，它的投资回报率（最环保的泡沫）是最好的。

>[!TIP]
>
>您可以快速将一个渠道中的项目与另一个渠道中的项目进行比较。 只需使用 **渠道筛选器** 以添加更多渠道。

>[!MORELIKETHIS]
>
>* [使用计划分析器浏览计划和渠道详细信息](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [使用项目分析器比较渠道有效性](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)
