---
unique-page-id: 2951877
description: 了解项目机会分析区域 — Marketo文档 — 产品文档
title: 了解计划机会分析领域
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# 了解计划机会分析领域 {#understanding-the-program-opportunity-analysis-area}

## 概述 {#overview}

计划机会分析区域允许您分析各个计划的有效性或查看按计划渠道列出的汇总结果。

**使用此分析区域可以回答的业务问题示例包括**：

与给定计划相关的机会有多少，我们赢得了多少机会？

![](assets/one-1.png)

某个节目或渠道帮助产生了多少收入？

![](assets/two-1.png)

对于给定的计划或渠道，我的投资收入是多少？

![](assets/three-1.png)

给定项目影响了哪些机会？

![](assets/four-1.png)

## 计划机会分析归因措施（蓝点） {#program-opportunity-analysis-attribution-measures-blue-dots}

可用于分析的测量通常为数字，并以蓝点表示。 Dimension是给出度量不同视图的属性，由黄点表示。

所有指标（蓝点）均与归因相关，即商机收购或与商机相关的销售成功的“点数”。

![](assets/six.five.png) ![](assets/seven-1.png)

有三种措施：

* 与收购相关的指标，即首次接触归因(FT)。
* 与成功相关的度量，此类度量会接收多点接触归因(MT)。
* 其他与项目群相关的度量，包括在创建或关闭业务机会之前的平均营销接触次数。

## 客户获取和成功相关措施 {#acquisition-and-success-related-measures}

与收购相关的措施为首次获取商机的联系信息的计划提供点数。 潜在客户不必在要授予的客户获取信用计划中取得成功。

获取给定潜在客户的价值会随着时间的推移而改变。 在潜在客户进行购买之前，该值为零。 然后，它会随着额外购买而增加。

与成功相关的措施将促进潜在客户购买进展的所有方案都归功于成功。

与收购一样，对销售线索的贡献值会随着时间的推移而改变，直到销售线索进行某些购买时该值才会为零。

<table> 
 <tbody> 
  <tr> 
   <th>Attribution Measure — 与机会相关（FT或MT）*</th> 
   <th>描述</th> 
  </tr> 
  <tr> 
   <td>机会成本</td> 
   <td>项目成本中影响机会的部分。 如果涉及多个潜在客户，则成本可以分摊。</td> 
  </tr> 
  <tr> 
   <td>已创建的机会</td> 
   <td>项目因影响机会的创造而获得的点数部分。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>赢得的机会</td> 
   <td>项目因影响成功的机会而获得的积分部分。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>管道已创建</td> 
   <td>计划因影响机会的创造而收到的信用部分（以货币价值表示）。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>管道已创建 — 仍然打开</td> 
   <td>计划收到的用于影响当前开放机会创建的信用部分（以货币价值表示）。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>预计收入</td> 
   <td>计划因影响机会的创造而收到的信用部分（以货币价值表示）。 预期收入是机会概率乘以机会值。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>投资收入</td> 
   <td>这是计划收到的用于影响成功的机会和计划成本的信贷部分（以货币价值表示）的比率。</td> 
  </tr> 
  <tr> 
   <td>赢得的收入</td> 
   <td>项目因影响成功的机会而获得的信用部分（以货币价值表示）。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) =首次接触归因，用于商机获取衡量；(MT) =多点接触归因，用于商机成功衡量_

以下方案描述了当有两个项目生成了销售线索，但这些销售线索从同一帐户生成了一个Opportunity时，如何计算Opportunity Units。

**方案1**

* 生成一个潜在客户：潜在客户1
* 潜在客户1来自帐户1

**项目2**

* 生成另一个潜在客户：潜在客户2
* 潜在客户2也来自客户1

**帐户1**

* 生成一个Opportunity： Opportunity 1

Marketo会适当地提供点数，而不会在项目间重复计算机会。 因此，在本例中，每个计划会收到0.5个机会单位。 也就是说，每个项目都会获得所生成Opportunity的一半信用。 另外，与Opportunity关联的一半收入分配给每个Program。

## 其他方案相关措施 {#miscellaneous-program-related-measures}

现有的其他措施反映了方案的总体执行情况。

<table> 
 <tbody> 
  <tr> 
   <th>归因衡量 — 项目相关</th> 
   <th>描述</th> 
  </tr> 
  <tr> 
   <td>与项目群相关的机会数</td> 
   <td><p>向项目群提供任何类型的归因点数的机会总数。 机会可能受一个或多个潜在客户以及一个或多个项目的影响。</p></td> 
  </tr> 
  <tr> 
   <td>每个已结束机会的平均成功数</td> 
   <td>Opportunity关闭前项目成功的平均数。 <br></td> 
  </tr> 
  <tr> 
   <td>每个创建的机会的平均成功数</td> 
   <td>创建Opportunity之前项目成功的平均数。</td> 
  </tr> 
  <tr> 
   <td>新名称</td> 
   <td>计划获得的新名称（即新商机）总数。</td> 
  </tr> 
  <tr> 
   <td>计划成本</td> 
   <td>计划的总成本。</td> 
  </tr> 
  <tr> 
   <td>成功（总计）</td> 
   <td>取得成功的计划成员总数。</td> 
  </tr> 
 </tbody> 
</table>

## Program Opportunity AnalysisDimension（黄点） {#program-opportunity-analysis-dimensions-yellow-dots}

虽然计算量度（蓝点）会计算并且需要一些思维和说明才能使用，但维度（黄点）是描述性的。 以下是可用的维度。

<table> 
 <tbody> 
  <tr> 
   <th>类别</th> 
   <th>显示标签</th> 
  </tr> 
  <tr> 
   <td>机会属性</td> 
   <td>机会已关闭<br>机会名称*<br>机会所有者名称<br>机会阶段<br>机会类型</td> 
  </tr> 
  <tr> 
   <td>机会时间范围</td> 
   <td>Opportunity Closed Year/Quarter/Month<br>Opportunity创建年份/季度/月</td> 
  </tr> 
  <tr> 
   <td>项目群属性</td> 
   <td>项目频道<br>项目名称</td> 
  </tr> 
  <tr> 
   <td>项目成本时间范围</td> 
   <td>成本年度/季度/月</td> 
  </tr> 
 </tbody> 
</table>

*&#42;将任何类型的归因点数提供给项目的所有机会。 机会可能受一个或多个潜在客户以及一个或多个项目的影响。*

>[!MORELIKETHIS]
>
>[创建收入浏览器报表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
