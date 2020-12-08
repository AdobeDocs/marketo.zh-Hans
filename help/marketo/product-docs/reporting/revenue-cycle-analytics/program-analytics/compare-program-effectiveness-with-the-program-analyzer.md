---
unique-page-id: 2360403
description: 将项目有效性与项目分析器— Marketo Docs —产品文档进行比较
title: 将项目有效性与项目分析器进行比较
translation-type: tm+mt
source-git-commit: f74d028e491aa70913fbe5cf14e536e50dbee32b
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---


# 将项目有效性与项目分析器进行比较 {#compare-program-effectiveness-with-the-program-analyzer}

通过比较项目成本、成员赢取、渠道和收入，使用项目分析器来识别最有效、最低效的项目。

>[!NOTE]
>
>**先决条件**
>
>* [创建项目分析器](create-a-program-analyzer.md)


1. 单击“Analytics（分析）”。

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 选择项目分析器。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 将视图更改为按项目。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. 使用渠道过滤器将视图减少到一两个渠道。 现在，我们来看展会渠道的项目。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >将项目筛选为仅一个渠道的快速方法是选择 **视图>按渠道**，单击该渠道的气泡，然后在弹出对话框中单击渠道名称。

1. 使用X轴下拉列表为水平轴选择度量。 我们用项目成本开始。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 使用Y轴下拉列表为垂直轴选择度量。 让我们选择“新名称”以查找擅长捕获新潜在客户的项目。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. 打开滑块进行放大。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >您还可以尝试通过从线性比例更改为对数比例来改善视图，反之亦然。 使用顶 **部的** “缩放”菜单。

1. 浏览结果图。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   在我们的例子中，我们了解到折纸展比渠道里的其他项目在捕捉新名字时要好得多，而且要以中等的成本。 但这不是全部。 我们将再添加两个指标，以加深理解。

1. 使用“气泡大小”下拉菜单选择要按气泡大小进行比较的度量。 我们将以(FT)赢取收入为例。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >在项目分析器中可以选择的许多指标可通过首次触控(FT)和多触(MT)计算获得。 了解FT与MT归因 [的区别很重要](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)。

1. 观察图中气泡的大小变化。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   通过加 **入(FT)Revenue Won**，我们很快发现，虽然“折纸展”获得了许多新的品牌，但它带来的收入相对较少。 此外，我们还看到，Paper Fest 12项目的名声越来越少，但越来越好，因为它影响了赢取的更多收入（更大的泡沫）。

1. 使用颜色下拉列表添加第四个度量。 我们来看(FT)投资收益。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. 观察图中的颜色变化。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

我们看到，Paper Fest 12项目不仅影响更多收入（更大的泡沫），而且尽管其项目成本相对较高（在最右边），但在展会渠道，它的投资回报（最环保的泡沫）是所有项目的最佳。

>[!TIP]
>
>您可以快速比较一个渠道中的项目与另一个中的数据。 只需使用 **窗口顶部的渠道** “过滤器”，即可添加更多渠道。

>[!NOTE]
>
>**相关文章**
>
>* [使用项目分析器了解渠道和项目详细信息](explore-program-and-channel-details-with-the-program-analyzer.md)
>* [将渠道有效性与项目分析器进行比较](compare-channel-effectiveness-with-the-program-analyzer.md)


>[!NOTE]
>
>了解有关收入周期浏览器中高级 [分析的更多信息](http://docs.marketo.com/display/docs/revenue+cycle+analytics)。
