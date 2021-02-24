---
unique-page-id: 2951877
description: 了解项目机会分析区域 — Marketo Docs — 产品文档
title: 了解项目机会分析区
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---


# 了解项目机会分析区域{#understanding-the-program-opportunity-analysis-area}

## 概述{#overview}

项目机会分析区域允许您分析各个项目的效率，或查看按项目渠道列出的汇总结果。

**您可以使用此分析区域回答的业务问题示例包括**:

有多少个Opportunities与特定项目关联，有多少个Opportunities与我们赢得？

![](assets/one-1.png)

特定项目或渠道帮助创造了多少收入？

![](assets/two-1.png)

对于给定项目或渠道，我的“收入对投资”是多少？

![](assets/three-1.png)

哪些机会对项目产生了影响？

![](assets/four-1.png)

## 项目机会分析归因度量（蓝点）{#program-opportunity-analysis-attribution-measures-blue-dots}

可用于分析的度量通常是数字，由蓝点表示。 Dimension是给出度量的不同视图的属性，由黄色圆点表示。

所有指标（蓝点）都与归因相关 — 潜在客户赢取或与潜在客户关联的销售成功的“信用”。

![](assets/six.five.png) ![](assets/seven-1.png)

有三种措施：

* 与收购相关的衡量指标，它们获得了首次接触归因(FT)。
* 成功相关措施，可接收多触归因(MT)。
* 与项目相关的其他度量，包括在创建或关闭Opportunity之前的平均营销接触次数。

## 收购和成功相关措施{#acquisition-and-success-related-measures}

与收购有关的措施给予首次获得潜在客户联系信息的项目信用。 潜在客户不必在要授予的收购信用项目中取得成功。

随着时间推移，获取给定潜在客户的值会发生变化。 在由潜在客户进行购买之前，它为零。 随后可随额外购买而增加。

成功相关措施为促成销售线索采购进展的所有项目提供了信誉。

与客户赢取一样，对销售所做贡献的价值会随着时间而改变，在销售线索进行某些购买之前为零。

<table> 
 <tbody> 
  <tr> 
   <th>归因度量 — 机会相关（FT或MT）*</th> 
   <th>说明</th> 
  </tr> 
  <tr> 
   <td>机会成本</td> 
   <td>影响机会的项目成本部分。 如果涉及多个潜在客户，则可能会分摊成本。</td> 
  </tr> 
  <tr> 
   <td>创建的机会</td> 
   <td>项目为影响机会创造而获得的信用部分。 如果涉及多个潜在客户，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>赢得了机会</td> 
   <td>项目为影响赢得的机会而收到的信用部分。 如果涉及多个潜在客户，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>已创建管线</td> 
   <td>为影响机会的创造而收到的信用部分（以货币价值计）项目。 如果涉及多个潜在客户，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>已创建管道 — 仍然打开</td> 
   <td>为影响当前开放机会的创造而收到的信用部分（以货币价值计）项目。 如果涉及多个潜在客户，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>预期收入</td> 
   <td>为影响机会的创造而收到的信用部分（以货币价值计）项目。 预期收入是机会概率乘以机会值。 如果涉及多个潜在客户，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>投资收益</td> 
   <td>这是为影响赢得的机会而收到的项目的信用部分（以货币价值计）与项目成本之比。</td> 
  </tr> 
  <tr> 
   <td>赢取收入</td> 
   <td>为影响赢得的机会而收到的项目的信用部分（以货币价值计）。 如果涉及多个潜在客户，这可能只是一小部分。</td> 
  </tr> 
 </tbody> 
</table>

_*(FT)=首次接触归因，用于铅的获取量度；(MT)=多触归因，用于衡量潜在客户成功与否_

下面是一个方案，其中描述了当有两个项目生成了潜在客户，但这些潜在客户从同一帐户中导致了一个Opportunity时，如何计算Opportunity Units。

**项目 1**

* 生成一个潜在客户：潜在客户1
* 潜在客户1来自帐户1

**项目 2**

* 生成另一个潜在客户：潜在客户2
* 潜在客户2也来自帐户1

**帐户1**

* 生成一个Opportunity:机会1

Marketo在不计多次的情况下为项目提供适当的信用。 因此，在本例中，每个项目接收0.5个机会单位。 也就是说，每个项目都会收到生成的Opportunity的一半信用。 此外，与Opportunity关联的一半收入被分配给每个项目。

## 杂项项目相关措施{#miscellaneous-program-related-measures}

现有的其他衡量指标反映了该项目的整体业绩。

<table> 
 <tbody> 
  <tr> 
   <th>归因度量 — 与项目相关</th> 
   <th>说明</th> 
  </tr> 
  <tr> 
   <td>与项目相关的机会数</td> 
   <td><p>给予项目任何类型归因的总Opportunity数。 机会可能受到一个或多个潜在客户以及一个或多个项目的影响。</p></td> 
  </tr> 
  <tr> 
   <td>每个已关闭机会的平均成功次数</td> 
   <td>在Opportunity关闭之前项目成功的平均数。 <br></td> 
  </tr> 
  <tr> 
   <td>每个已创建机会的平均成功次数</td> 
   <td>创建Opportunity之前项目成功的平均数。</td> 
  </tr> 
  <tr> 
   <td>新名称</td> 
   <td>由项目获取的新名称（即新潜在客户）的总数。</td> 
  </tr> 
  <tr> 
   <td>项目成本</td> 
   <td>项目总成本。</td> 
  </tr> 
  <tr> 
   <td>成功（总计）</td> 
   <td>成功的项目成员总数。</td> 
  </tr> 
 </tbody> 
</table>

## 项目机会分析Dimension（黄点）{#program-opportunity-analysis-dimensions-yellow-dots}

度量（蓝点）是计算的，需要一些思考和解释才能使用，而尺寸（黄点）是描述性的。 以下是可用维度。

<table> 
 <tbody> 
  <tr> 
   <th>类别</th> 
   <th>显示标签</th> 
  </tr> 
  <tr> 
   <td>机会属性</td> 
   <td>Opportunity Closed <br> Opportunity Name*<br> Opportunity Owner Name<br> Opportunity Stage<br> Opportunity Type</td> 
  </tr> 
  <tr> 
   <td>机会时间范围</td> 
   <td>已结业务机会年度/季度/月<br>已创建业务机会年度/季度/月</td> 
  </tr> 
  <tr> 
   <td>项目属性</td> 
   <td>项目渠道<br>项目名称</td> 
  </tr> 
  <tr> 
   <td>项目成本时间范围</td> 
   <td>成本年/季度/月</td> 
  </tr> 
 </tbody> 
</table>

**为项目提供任何类型归因的所有Opportunity。机会可能受一个或多个潜在客户和一个或多个项目的影响。*

>[!MORELIKETHIS]
>
>[创建收入浏览器报表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
