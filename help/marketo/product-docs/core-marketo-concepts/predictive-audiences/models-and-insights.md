---
description: 模型和见解 — Marketo文档 — 产品文档
title: 模型与洞察
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# 模型与洞察 {#models-and-insights}

模型的性能取决于输入数据的质量和完整性。 查看每个可能性AI模型的最大影响因素。 此外，还可了解导致活动注册率、活动出席率或取消订阅率提高/降低的前几个因素。

>[!NOTE]
>
>标有(+)的行为会对预测产生正向影响（反之亦然）。

下面是如何评估您模型的健康情况的。

导航到Marketo Engage **[!UICONTROL Models and Data Health]**&#x200B;区域的&#x200B;**[!UICONTROL Predictive Audiences]**&#x200B;下的&#x200B;**[!UICONTROL Admin]**&#x200B;部分。 在这里，您将看到您的所有模型及其状态。

![图像1](assets/models-and-insights-1.png)

* **训练状态**：指示模型是否正在积极训练（改进预测）。 每两周自动进行一次培训。 任何处于&#x200B;_处理_&#x200B;状态的模型最多可能需要24小时才能完成。 对于任何&#x200B;_失败_&#x200B;模型，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}。
* **评分状态**：指示模型是否正在主动计算计划成员的预测（可能性百分比）。
* **性能**：根据数据完整性和数据质量对模型运行状况进行分类（请参阅下文）。
* **数据完整性**：存在/完成的数据属性的百分比。
* **数据质量**：包含良好可用数据的属性的百分比。
* **上次训练时间**：当前模型与每两周训练一次的新模型之间在评估中表现最佳的模型日期。
