---
unique-page-id: 2951877
description: 了解计划机会分析区域 — Marketo文档 — 产品文档
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

**您可以使用此分析区域回答的业务问题示例包括**：

与给定计划相关的机会有多少，我们赢得了多少机会？

![](assets/one-1.png)

一个给定的计划或渠道帮助产生了多少收入？

![](assets/two-1.png)

对于给定的计划或渠道，我的投资收入是多少？

![](assets/three-1.png)

给定项目影响了哪些机会？

![](assets/four-1.png)

## 计划机会分析归因措施（蓝点） {#program-opportunity-analysis-attribution-measures-blue-dots}

可用于分析的测量通常为数字，并以蓝点表示。 Dimension是提供各种度量视图的属性，用黄点表示。

所有指标（蓝点）都与归因相关，即潜在客户获取或与潜在客户关联的销售成功的“点数”。

![](assets/six.five.png) ![](assets/seven-1.png)

有三种措施：

* 获得首次接触归因(FT)的收购相关指标。
* 与成功相关的度量，此类度量会接收多点接触归因(MT)。
* 其他与项目群相关的衡量标准，包括创建或关闭业务机会之前的营销接触平均数量。

## 客户获取和成功相关措施 {#acquisition-and-success-related-measures}

与收购相关的措施为首次获取潜在客户联系信息的计划提供点数。 潜在客户不必在要授予的获取信用计划中取得成功。

获取给定商机的值会随时间而改变。 在潜在客户进行购买之前，该值为零。 然后，它会随着额外购买而增加。

与成功相关的措施将功劳归于有助于潜在客户在购买方面取得进展的所有计划。

与收购时一样，对销售线索的贡献值会随着时间而改变，并且直到销售线索进行某些购买之前为零。

<table> 
 <tbody> 
  <tr> 
   <th>归因指标 — 与机会相关（FT或MT）*</th> 
   <th>描述</th> 
  </tr> 
  <tr> 
   <td>机会成本</td> 
   <td>项目成本中影响机会的部分。 如果涉及多个潜在客户，则成本可以分摊。</td> 
  </tr> 
  <tr> 
   <td>机会已创建</td> 
   <td>计划因影响机会的创造而获得的功劳部分。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>赢得的机会</td> 
   <td>计划因影响赢得的机会而获得的积分部分。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>管道已创建</td> 
   <td>计划因影响机会的创造而获得的信贷部分（以货币价值表示）。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>管道已创建 — 仍然打开</td> 
   <td>计划因影响当前开放机会的创造而获得的信贷部分（以货币价值表示）。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>预期收入</td> 
   <td>计划因影响机会的创造而获得的信贷部分（以货币价值表示）。 预期收入是机会概率乘以机会值。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>投资收入</td> 
   <td>这是项目因影响成功的机会和项目成本而获得的信贷部分（以货币价值表示）的比率。</td> 
  </tr> 
  <tr> 
   <td>赢得的收入</td> 
   <td>计划因影响赢得的机会而获得的信用部分（以货币价值表示）。 如果涉及多个线索，则可能只是一小部分。</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) =首次接触归因，用于评估商机收购情况；(MT) =多点接触归因，用于评估商机是否成功_

以下情形描述了当存在两个生成潜在客户的项目时，如何计算Opportunity Units ，但是这些潜在客户会从同一帐户生成一个Opportunity。

**项目1**

* 生成一个潜在客户：潜在客户1
* 潜在客户1来自帐户1

**项目2**

* 生成另一个潜在客户：潜在客户2
* 潜在客户2也来自客户1

**帐户1**

* 生成一个Opportunity： Opportunity 1

Marketo会适当地提供点数，而不会在项目间重复计算Opportunity。 因此，在此例中，每个计划收到0.5个机会单位。 也就是说，每个计划都会获得所生成Opportunity一半的点数。 另外，与Opportunity关联的一半收入分配给每个Program。

## 与方案有关的杂项措施 {#miscellaneous-program-related-measures}

其他现有措施反映了该方案的总体执行情况。

<table> 
 <tbody> 
  <tr> 
   <th>归因衡量标准 — 项目群相关</th> 
   <th>描述</th> 
  </tr> 
  <tr> 
   <td>与项目群相关的机会数</td> 
   <td><p>为项目提供任何类型的归因点数的“机会”总数。 机会可能受一个或多个潜在客户以及一个或多个项目的影响。</p></td> 
  </tr> 
  <tr> 
   <td>每个已结束机会的平均成功数</td> 
   <td>Opportunity关闭前计划成功项目的平均数量。 <br></td> 
  </tr> 
  <tr> 
   <td>每个创建的机会的平均成功数</td> 
   <td>创建Opportunity之前成功项目的平均数量。</td> 
  </tr> 
  <tr> 
   <td>新名称</td> 
   <td>计划获得的新名称（即新商机）总数。</td> 
  </tr> 
  <tr> 
   <td>计划成本</td> 
   <td>计划总成本。</td> 
  </tr> 
  <tr> 
   <td>成功（总计）</td> 
   <td>取得成功的计划成员总数。</td> 
  </tr> 
 </tbody> 
</table>

## Program Opportunity AnalysisDimension（黄点） {#program-opportunity-analysis-dimensions-yellow-dots}

虽然量度（蓝点）是计算的，并且需要一些思维和解释才能使用，但维度（黄点）是描述性的。 以下是可用的维度。

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
   <td>计划渠道<br>项目名称</td> 
  </tr> 
  <tr> 
   <td>计划成本时间范围</td> 
   <td>成本年度/季度/月</td> 
  </tr> 
 </tbody> 
</table>

*&#42;将任何类型的归因点数提供给项目的所有机会。 机会可能受一个或多个潜在客户以及一个或多个项目的影响。*

>[!MORELIKETHIS]
>
>[创建收入资源管理器报表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
