---
description: 产品使用情况功能板 — Marketo文档 — 产品文档
title: 产品使用情况功能板
hide: true
hidefromtoc: true
feature: Administration
exl-id: a0fa5cd0-a61d-4383-88c0-9f2a4b2c717a
source-git-commit: d7a7e6f7fd9c9009a058578f6027698a181226f5
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 产品使用情况功能板 {#product-usage-dashboards}

Marketo Engage产品使用情况功能板能够根据某些限制或积压的数据吞吐量、每日配额的使用情况以及订阅中的关键量度查看产品和平台使用情况。 分配基础结构是为了提供为特定属性的产品级别定义的性能限制。 其中一些限制（如API使用）是作为包或产品层的一部分购买的合同限制。

## 如何访问 {#how-to-access}

1. 在Marketo Engage中，单击&#x200B;**管理员**。

   ![](assets/product-usage-dashboards-1.png)

1. 在左侧的树中，向下滚动并选择&#x200B;**产品使用情况仪表板**。

   ![](assets/product-usage-dashboards-2.png)

## 活动使用情况仪表板 {#activity-usage-dashboard}

### 每周平均活动 {#average-weekly-activities}

“每周活动使用情况”功能板提供连续52周内的活动类型每周计数。 每周生成的活动可很好地指示您在Marketo Engage中进行多少营销。 活动充当在Marketo内发生的各种系统进程和可跟踪事件的代理。

活动类型包括人员/商机与营销事件交互时捕获的活动计数，以及由流操作触发的基于系统的活动。 人员启动活动的一些示例包括：收件人打开您发送的电子邮件，或单击电子邮件中的链接时。 流程操作所触发的基于系统的活动的示例为：在触发程序启动时&#x200B;_发送到SFDC_。

>[!TIP]
>
>要查看特定周的活动类型计数，请将鼠标悬停在所需的一周上，此时将显示该计数。

![](assets/product-usage-dashboards-3.png){width="800" zoomable="yes"}

#### 常见问题解答 {#faq}

**计算哪些活动类型？**

这取决于管道中包含哪些活动。

**包含已知和匿名人员/潜在客户活动？**

仅已知的人员/潜在客户。

**数据刷新频率如何？**

活动计数每天早上都会刷新。

## 活动细分 {#activity-breakdown}

在这里，我们根据数据的有意义的切片获取过去七天的活动计数。 按过去七天内出现的最常见活动类型对活动进行分组。 这可能包括&#x200B;_更改数据值_、_添加到列表_&#x200B;或&#x200B;_发送电子邮件_&#x200B;等类别。 这使您能够查看系统中最常发生的活动类型。 活动类型使用率是确定增长或是否需要进行优化以减少使用量的关键指标。

>[!NOTE]
>
>* 以下所有细分都是七天滚动总计，并且&#x200B;**不**&#x200B;包含当天。 所以可以把它想成是“昨天+六天前”
>
>* 仪表板仅显示前20个活动类型，而其余活动类型分类为名为“其他”的类别。

活动使用情况可向您显示正在进行多少营销，并有助于对照已订约产品级别确定的增长，实现可视化。 仪表板还可用作指南，以确定通过减少所更新的字段可以/应该进行多少优化。

### 按类型 {#by-type}

按过去七天内出现的最常见活动类型对活动进行分组。 这可能包括&#x200B;_更改数据值_、_添加到列表_&#x200B;或&#x200B;_发送电子邮件_&#x200B;等类别。 这使您能够查看Marketo Engage帐户中经常发生哪些类型的活动。

![](assets/product-usage-dashboards-4.png){width="600" zoomable="yes"}


### 通过更改数据值属性 {#by-change-data-value-attribute}

_更改数据值_&#x200B;是最常见的活动类型。 它指示人员/潜在客户记录中的一段信息何时更新。 在本例中，我们按照更改最频繁的字段进行分组，以便您可以确定哪些信息对营销操作有用、是否有机会优化平台使用情况等。

![](assets/product-usage-dashboards-5.png){width="600" zoomable="yes"}

### 按营销活动 {#by-campaign}

营销活动在其中产生最多活动的组。 这样，您就可以查看是否存在任何特别“嘈杂”的营销活动，这些营销活动会创建超出所需数量的活动。 快速了解应停用的营销活动或完成的工作超出预期营销活动。

![](assets/product-usage-dashboards-6.png){width="600" zoomable="yes"}
