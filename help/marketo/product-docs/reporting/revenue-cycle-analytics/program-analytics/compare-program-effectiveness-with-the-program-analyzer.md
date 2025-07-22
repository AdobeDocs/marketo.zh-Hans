---
unique-page-id: 2360403
description: 使用程序分析器比较程序有效性 — Marketo文档 — 产品文档
title: 使用程序分析器比较程序有效性
exl-id: 6e54d0a4-3cff-46cf-be0d-1992a39d8c03
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 将计划效果与[!UICONTROL Program Analyzer]进行比较 {#compare-program-effectiveness-with-the-program-analyzer}

使用[!UICONTROL Program Analyzer]通过比较项目成本、成员获取、管道和收入，确定您最有效和最不有效的项目。

>[!PREREQUISITES]
>
>[创建[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 单击 **[!UICONTROL Analytics]**。

   ![](assets/image2014-9-17-18-3a50-3a30.png)

1. 选择程序分析器。

   ![](assets/image2014-9-17-18-3a50-3a37.png)

1. 将视图更改为&#x200B;**[!UICONTROL By Program]**。

   ![](assets/image2014-9-17-18-3a50-3a44.png)

1. 使用&#x200B;**[!UICONTROL Channel Filter]**&#x200B;将视图缩小到仅一个或两个通道。 现在，我们将查看&#x200B;**[!UICONTROL Tradeshow]**&#x200B;频道中的节目。

   ![](assets/image2014-9-17-18-3a51-3a2.png)

   >[!TIP]
   >
   >将程序筛选为仅包含一个渠道的快速方法是选择&#x200B;**[!UICONTROL View]** > **[!UICONTROL By Channel]**，单击该渠道的气泡，然后在弹出对话框中单击渠道名称。

1. 使用&#x200B;**[!UICONTROL X Axis]**&#x200B;下拉菜单选择水平轴的量度。 我们将从&#x200B;**[!UICONTROL Program Cost]**&#x200B;开始。

   ![](assets/image2014-9-17-18-3a52-3a16.png)

1. 使用&#x200B;**[!UICONTROL Y Axis]**&#x200B;下拉菜单选择垂直轴的量度。 让我们选择&#x200B;**[!UICONTROL New Names]**&#x200B;以查找擅长捕获新商机的程序。

   ![](assets/image2014-9-17-18-3a52-3a26.png)

1. 打开滑块以放大。

   ![](assets/image2014-9-17-18-3a53-3a9.png)

   >[!TIP]
   >
   >您也可以尝试通过从线性缩放更改为对数缩放来改善视图，反之亦然。 使用顶部的&#x200B;**[!UICONTROL Scale]**&#x200B;菜单。

1. 浏览生成的图表。

   ![](assets/image2014-9-17-18-3a53-3a49.png)

   在我们的示例中，我们了解[!DNL Origami Expo]在捕获新名称方面远远优于该渠道中的所有其他程序，并且成本适中。 但这不是故事的全部。 我们将再添加两个量度以加深了解。

1. 使用&#x200B;**[!UICONTROL Bubble Size]**&#x200B;下拉菜单选择要按气泡大小比较的量度。 我们将选择&#x200B;**[!UICONTROL (FT) Revenue Won]**&#x200B;作为示例。

   ![](assets/image2014-9-17-18-3a54-3a25.png)

   >[!NOTE]
   >
   >您可以在程序分析器中选择的许多量度都可用于首次联系(FT)和多点联系(MT)计算。 了解FT和MT归因[之间的](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)差异很重要。

1. 观看图表中的气泡变化大小。

   ![](assets/image2014-9-17-18-3a54-3a57.png)

   通过添加&#x200B;**[!UICONTROL (FT) Revenue Won]**，我们很快发现，虽然[!DNL Origami Expo]获得了许多新名称，但产生的收入相对较少。 此外，我们看到[!DNL Paper Fest 12]项目越来越少，但名称越来越好，因为它会影响赢得的更多收入（更大的气泡）。

1. 使用颜色下拉菜单添加第四个量度。 我们将查看&#x200B;**[!UICONTROL (FT) Revenue to Investment]**。

   ![](assets/image2014-9-17-18-3a55-3a33.png)

1. 观察图形中的颜色变化。

   ![](assets/image2014-9-17-18-3a55-3a47.png)

我们看到[!DNL Paper Fest 12]计划不仅会影响更多收入（更大的泡沫），而且尽管其计划成本相对较高（位于最右边），但其投资回报率（最环保的泡沫）是[!UICONTROL Tradeshow]渠道中所有计划的最佳回报。

>[!TIP]
>
>您可以快速将一个渠道中的项目与另一个渠道中的项目进行比较。 只需使用窗口顶部的&#x200B;**渠道筛选器**&#x200B;添加更多渠道即可。

>[!MORELIKETHIS]
>
>* [使用[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)浏览计划和渠道详细信息
>* [将渠道效果与[!UICONTROL Program Analyzer]](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-channel-effectiveness-with-the-program-analyzer.md)进行比较
