---
unique-page-id: 2360401
description: 将渠道有效性与项目分析器— Marketo Docs —产品文档进行比较
title: 将渠道有效性与项目分析器进行比较
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---


# 将渠道有效性与项目分析器进行比较 {#compare-channel-effectiveness-with-the-program-analyzer}

使用项目分析器比较渠道成本、成员获取、渠道、收入等，以确定最有效、最不有效的渠道。

>[!PREREQUISITES]
>
>* [创建项目分析器](create-a-program-analyzer.md)


1. 单击“ **My** Marketo **”中的Analytics。**

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 选择您的 **项目分析器。**

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 将视图更改为 **按****渠道**。

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 使用 **X轴** （X轴）下拉框选择水平轴的度量。 让我们用开始成 **本项目**。

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. 使用Y轴下拉列表为垂直轴选择度量。 这里，我们将介绍(FT) **创建的管道**。

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >在项目分析器中可以选择的许多指标可通过首次触控(FT)和多触(MT)计算获得。 了解FT与MT归因 [的区别很重要](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)。

1. 使用 **Y轴下拉** ，选择“( **MT)已创建管线”**。

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   在此多触归因视图中，我们发现网络研讨会渠道对创建的渠道的影响更大，并且比贸易展和在线广告渠道的成本更低。

   现在，我们再添加两个维度！

1. 使用“ **气泡大小** ”下拉框选择其他度量，如“ **新名称”**。

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. 观看图表的变化。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   我们看到网络研讨会渠道会缩小，用新名称 **来衡量**。 我们可以得出这样的结论：尽管它拥有许多成员，但它在创造新线索方面不如贸易展渠道有效。

1. 最后，使用“颜色”(Color)下拉框添加第四个维度。 让我们选 **择(FT)收入****赢**。

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. 观察图中的颜色变化。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   从色彩上，我们了解到，作为最绿色的泡沫，展会渠道影响了最大的收益，这是通过首次接触归因衡量的。

1. 现在，如果我们将颜色指标更改为( **MT)收入赢得**，我们会发现，与网络研讨会和贸易展渠道相比，在线广告渠道（现在是最环保的）影响了更多的收入。

   ![](assets/image2014-9-17-18-3a41-3a40.png)

在我们的示例中，我们看到展会渠道在测量首次触摸创建的管道时既最昂贵（最右边），也最成功（Y轴最高）。 现在，让我们考虑一下每个渠道创建的管道是通过多点触控归因来衡量的。

>[!TIP]
>
>这些步骤中的示例根据创建的管道衡量有效性。 使用Y轴下拉列表选择其他衡量渠道有效性的方法，如新名称、成员、每次成功的成本等。

>[!NOTE]
>
>**相关文章**
>
>* [使用项目分析器了解渠道和项目详细信息](explore-program-and-channel-details-with-the-program-analyzer.md)
>* [将项目有效性与项目分析器进行比较](compare-program-effectiveness-with-the-program-analyzer.md)

>



>[!NOTE]
>
>了解有关收入周期浏览器中高级 [分析的更多信息](http://docs.marketo.com/display/docs/revenue+cycle+analytics)。
