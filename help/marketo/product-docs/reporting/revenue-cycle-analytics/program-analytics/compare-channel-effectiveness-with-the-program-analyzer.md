---
unique-page-id: 2360401
description: 使用项目分析器比较渠道有效性 — Marketo文档 — 产品文档
title: 使用项目分析器比较渠道有效性
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 使用项目分析器比较渠道有效性 {#compare-channel-effectiveness-with-the-program-analyzer}

使用Program Analyzer比较渠道成本、成员获取、渠道、收入等，以确定最有效和最不有效的渠道。

>[!PREREQUISITES]
>
>[创建程序分析器](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. 在&#x200B;**我的Marketo**&#x200B;中单击&#x200B;**Analytics**。

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. 选择您的&#x200B;**程序分析器**。

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. 按渠道&#x200B;**将视图更改为**。

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. 使用&#x200B;**X轴**&#x200B;下拉菜单选择水平轴的量度。 让我们从&#x200B;**计划成本**&#x200B;开始。

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. 使用Y轴下拉菜单选择垂直轴的量度。 在此，我们将创建&#x200B;**（英尺）管道**。

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >您可以在程序分析器中选择的许多量度都可用于首次联系(FT)和多点联系(MT)计算。 了解FT和MT归因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md)之间的[差异很重要。

1. 使用&#x200B;**Y轴**&#x200B;下拉列表选择已创建的&#x200B;**(MT)管道**。

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   在此多点接触归因视图中，我们看到网络研讨会渠道对创建管道的影响比贸易展和在线Advertising渠道更大，成本更低。

   现在，让我们再添加两个维度！

1. 使用&#x200B;**气泡大小**&#x200B;下拉列表选择其他度量值，如&#x200B;**新名称**。

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. 观察图表如何变化。

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   我们看到网络研讨会渠道缩小了，如&#x200B;**新名称**&#x200B;所衡量。 我们可以得出这样的结论：尽管它拥有众多成员，但它在创造新的商机方面不如贸易展览渠道有效。

1. 最后，使用颜色下拉菜单添加第四个维度。 让我们选择&#x200B;**（英尺）收入**。

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. 观察图形中的颜色变化。

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   从颜色中，我们了解到，贸易展览渠道（最环保的泡沫）影响了获得的最大收入，这是通过首次接触归因来衡量的。

1. 现在，如果我们将颜色量度更改为&#x200B;**(MT)收入**，我们就会发现，现在最环保的在线Advertising渠道随着时间的推移对收入的影响比网络研讨会和商展渠道大。

   ![](assets/image2014-9-17-18-3a41-3a40.png)

在本例中，我们看到在测量由首次接触创建的管道时，贸易展览渠道最昂贵（最靠右）且最成功（在Y轴上最高）。 现在，让我们考虑按多接触点归因衡量的方式创建每个渠道的管道。

>[!TIP]
>
>这些步骤中的示例根据创建的管道来衡量有效性。 使用Y轴下拉列表选择衡量渠道效果的其他方法，如新名称、成员、每次成功成本等。

>[!MORELIKETHIS]
>
>* [使用计划分析器浏览计划和渠道详细信息](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [将计划效果与计划分析器进行比较](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)
