---
unique-page-id: 2951877
description: 了解项目机会分析区- Marketo Docs —— 产品文档
title: 了解项目机会分析区
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---


# 了解项目机会分析区 {#understanding-the-program-opportunity-analysis-area}

## 概述 {#overview}

项目机会分析区域允许您分析各个项目的有效性或按项目渠道查看汇总结果。

**您可以使用此分析区域回答的业务问题示例包括：**

有多少个Opportunities与特定项目相关，有多少个我们赢得了？

![](assets/one-1.png)

特定项目或渠道的收入有多少？

![](assets/two-1.png)

对于特定项目或渠道，我的投资收益是多少？

![](assets/three-1.png)

哪些机会对项目产生了影响？

![](assets/four-1.png)

## 项目机会分析归因度量（蓝点） {#program-opportunity-analysis-attribution-measures-blue-dots}

分析中可用的度量通常是数字，用蓝点表示。 Dimension是给出不同视图度量的属性，由黄色圆点表示。

所有衡量标准（蓝点）都与归因相关——潜在客户赢取或与潜在客户相关的销售成功的“信用”。

![](assets/six.five.png) ![](assets/seven-1.png)

有三种措施：

* 与客户赢取相关的衡量指标，它们获得首次接触归因(FT)。
* 成功相关指标，可接收多触归因(MT)。
* 与项目相关的其他衡量指标，包括创建或关闭Opportunity之前的平均营销接触次数。

## 赢取与成功相关的措施 {#acquisition-and-success-related-measures}

与收购相关的措施会归功于首次获得潜在客户联系信息的项目。 潜在客户不必在要授予收购信用的项目取得成功。

随时间推移，获取给定潜在客户的值会发生变化。 在由潜在客户进行购买之前，它为零。 然后，随着额外购买量的增加，它会增加。

与成功相关的衡量标准可以肯定促成潜在客户购买过程的所有项目。

与客户赢取一样，销售线索的销售贡献价值会随着时间的推移而改变，在潜在客户进行某些购买之前为零。

<table> 
 <tbody> 
  <tr> 
   <th>归因度量——机会相关（FT或MT）*</th> 
   <th>说明</th> 
  </tr> 
  <tr> 
   <td>机会成本</td> 
   <td><p>影响机会的项目成本部分。 如果涉及多个潜在客户，则成本可能会分摊。</p></td> 
  </tr> 
  <tr> 
   <td>创建的机会</td> 
   <td><p>项目因影响机会的创造而获得的信用部分。 如果涉及多个线索，这可能只是一小部分。</p></td> 
  </tr> 
  <tr> 
   <td>赢得机会</td> 
   <td>项目因影响赢得的机会而获得的信用部分。 如果涉及多个线索，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td>创建管道</td> 
   <td><p>用于影响机会创造的项目的信用部分（以货币价值计）。 如果涉及多个线索，这可能只是一小部分。</p></td> 
  </tr> 
  <tr> 
   <td>已创建管道——仍然打开</td> 
   <td>为影响当前开放机会的创造而收到的信用部分（以货币价值计）项目。 如果涉及多个线索，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td><p>预期收入</p></td> 
   <td>用于影响机会创造的项目的信用部分（以货币价值计）。 预期收入是机会概率乘以机会价值。 如果涉及多个线索，这可能只是一小部分。</td> 
  </tr> 
  <tr> 
   <td><p>投资收益</p></td> 
   <td><p>这是项目为影响赢得的机会而获得的信用部分（以货币价值计）与项目成本的比率。</p></td> 
  </tr> 
  <tr> 
   <td>赢得收入</td> 
   <td><p>为影响赢得的机会而收到的项目的信用部分（以货币价值计）。 如果涉及多个线索，这可能只是一小部分。</p></td> 
  </tr> 
 </tbody> 
</table>

**(FT)=首次接触归因，用于铅的获取计量；(MT)=多触归因，用于衡量潜在客户成功与否*

下面是一个方案，描述当有两个项目生成了潜在客户，但这些潜在客户从同一帐户生成了一个Opportunity时，如何计算Opportunity Unit。

**项目1**

* 生成一个潜在客户：潜在客户1
* 潜在客户1来自帐户1

**项目2**

* 生成另一个潜在客户：潜在客户2
* 潜在客户2也来自帐户1

**帐户1**

* 生成一个Opportunity:机会1

Marketo在不计多次的情况下为项目提供适当的信用机会。 因此，在本例中，每个项目都收到0.5个机会单位。 也就是说，每个项目都会收到生成的Opportunity的一半信用。 此外，与Opportunity关联的收入的一半分配给每个项目。

## 与项目有关的杂项措施 {#miscellaneous-program-related-measures}

现有的其他衡量标准反映了项目的总体业绩。

<table> 
 <tbody> 
  <tr> 
   <th>归因度量——与项目相关</th> 
   <th>说明</th> 
  </tr> 
  <tr> 
   <td>与项目相关的机会数</td> 
   <td><p>给予项目任何类型归因的Opportunity总数。 机会可能受到一个或多个线索以及一个或多个项目的影响。</p></td> 
  </tr> 
  <tr> 
   <td>每个已关闭机会的平均成功次数</td> 
   <td>在Opportunity关闭之前项目成功的平均数。 <br></td> 
  </tr> 
  <tr> 
   <td>每个机会创建的平均成功次数</td> 
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

## 项目机会分析Dimension（黄点） {#program-opportunity-analysis-dimensions-yellow-dots}

度量（蓝点）是计算的，需要一些思考和解释才能使用，而维（黄点）是描述性的。 以下是可用尺寸。

<table> 
 <tbody> 
  <tr> 
   <th>类别</th> 
   <th><p>显示标签</p></th> 
  </tr> 
  <tr> 
   <td>机会属性</td> 
   <td><p>Opportunity<br>ClosedOpportunity Name*<br>Opportunity Owner<br>NameOpportunity<br>StageOpportunity类型</p></td> 
  </tr> 
  <tr> 
   <td>机会时间范围</td> 
   <td><p>Opportunity Closed Year/Quarter/<br>MonthOpportunity Created Year/Quarter/Month</p></td> 
  </tr> 
  <tr> 
   <td>项目属性</td> 
   <td><p>项目<br>渠道计划名称</p></td> 
  </tr> 
  <tr> 
   <td>项目成本时间范围</td> 
   <td>成本年／季度／月</td> 
  </tr> 
 </tbody> 
</table>

**为项目提供任何类型归因的所有Opportunity。 机会可能受到一个或多个线索以及一个或多个项目的影响。*

>[!NOTE]
>
>**相关文章**
>
>[创建收入浏览器报表](../../../../product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
