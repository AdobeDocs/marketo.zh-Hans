---
unique-page-id: 2360401
description: 将渠道有效性与项目分析器 — Marketo Docs — 产品文档进行比较
title: 将渠道有效性与项目分析器进行比较
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# 将渠道有效性与项目分析器{#compare-channel-effectiveness-with-the-program-analyzer}比较

使用项目分析器比较渠道成本、成员赢取、渠道、收入等，以确定您最有效、最不有效的渠道。

>[!PREREQUISITES]
>
>[创建项目分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 单击&#x200B;**My Marketo**&#x200B;中的&#x200B;**Analytics**。

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 选择&#x200B;**项目分析器**。

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 将视图更改为&#x200B;**按渠道**。

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 使用&#x200B;**X轴**&#x200B;下拉列表为水平轴选择量度。 让我们用&#x200B;**项目成本**&#x200B;进行开始。

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. 使用Y轴下拉列表为垂直轴选择量度。 此处，我们将使用&#x200B;**(FT)Pipeline Created**。

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >在项目分析器中可以选择的许多量度都可进行首次触控(FT)和多触(MT)计算。 了解FT和MT归因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)之间的[差异非常重要。

1. 使用&#x200B;**Y轴**&#x200B;下拉框选择&#x200B;**(MT)已创建的管道**。

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   在此多触归因视图中，我们发现网络研讨会渠道对创建的渠道的影响力更大，并且比贸易展和在线广告渠道的成本更低。

   现在，让我们再添加两个维度！

1. 使用&#x200B;**气泡大小**&#x200B;下拉框选择其他度量，如&#x200B;**新名称**。

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. 观察图表的变化。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   我们看到网络研讨会渠道会缩小，用&#x200B;**新名称**&#x200B;来衡量。 我们可以得出结论，尽管它有很多成员，但它在创造新线索方面不如贸易展渠道有效。

1. 最后，使用“颜色”(Color)下拉框添加第四个尺寸。 让我们选择&#x200B;**(FT)收入原值**。

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. 观察图中的颜色变化。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   从颜色中，我们了解到，作为最绿色的泡沫，展会渠道对赢得的最大收入产生了影响，这是通过首次接触归因来衡量的。

1. 现在，如果我们将“颜色”量度更改为&#x200B;**(MT)收入赢**，我们会发现，与网络研讨会和展会渠道相比，现在最环保的在线广告渠道对收入的影响更大。

   ![](assets/image2014-9-17-18-3a41-3a40.png)

在我们的示例中，我们看到在测量由首次触控创建的管道时，展会渠道既是最昂贵（最右边），也最成功（Y轴最高）。 现在，让我们考虑一下每个渠道创建的管道是通过多触归因来衡量的。

>[!TIP]
>
>这些步骤中的示例根据创建的管道来衡量有效性。 使用Y轴下拉列表选择其他衡量渠道有效性的方法，如新名称、成员、每次成功的成本等。

>[!MORELIKETHIS]
>
>* [使用项目分析器了解渠道和项目详细信息](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [将项目有效性与项目分析器进行比较](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)

