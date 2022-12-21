---
unique-page-id: 2951877
description: 了解计划机会分析区域 — Marketo文档 — 产品文档
title: 了解计划机会分析领域
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# 了解计划机会分析领域 {#understanding-the-program-opportunity-analysis-area}

## 概述 {#overview}

通过“计划机会分析”区域，可以分析各个计划的有效性或按计划渠道查看总结结果。

**使用此分析区域可以回答的业务问题示例包括**:

有多少机会与给定的计划相关联，有多少机会与我们赢得了？

![](assets/one-1.png)

给定的计划或渠道有助于产生多少收入？

![](assets/two-1.png)

给定项目或渠道的我的投资收入是多少？

![](assets/three-1.png)

给定的项目对哪些机会有影响？

![](assets/four-1.png)

## 计划机会分析归因度（蓝点） {#program-opportunity-analysis-attribution-measures-blue-dots}

可用于分析的度量通常为数字，由蓝色圆点表示。 Dimension是一些属性，可提供不同的度量视图，并以黄色圆点表示。

所有指标（蓝点）都与归因相关 — 潜在客户获取或与潜在客户关联的销售成功的“点数”。

![](assets/six.five.png) ![](assets/seven-1.png)

有三种措施：

* 与客户获取相关的衡量指标，它们获得首次联系归因(FT)。
* 与成功相关的度量，可接收多接触归因(MT)。
* 与其他项目相关的措施，包括在创建或关闭Opportunity之前的平均营销接触次数。

## 收购和成功相关措施 {#acquisition-and-success-related-measures}

与收购相关的措施将归功于首次获得领导联系信息的方案。 在要授予的客户获取信用计划中，潜在客户不必取得成功。

随着时间推移，获取给定潜在客户的值会发生更改。 直到顾客购买商品为止，价格为零。 随后，随着额外购买的增加，流量会增加。

与成功相关的措施将归功于所有有助于销售线索实现购买的计划。

与客户获取一样，对潜在客户进行销售的贡献价值会随着时间的推移而发生变化，在潜在客户进行某些购买之前，该值为零。

<table> 
 <tbody> 
  <tr> 
   <th>归因度量 — 与机会相关（FT或MT）*</th> 
   <th>描述</th> 
  </tr> 
  <tr> 
   <td>机会成本</td> 
   <td>影响机会的计划成本部分。 如果涉及多个潜在客户，则成本可能会被分摊。</td> 
  </tr> 
  <tr> 
   <td>创建的机会</td> 
   <td>该方案为影响机会创造而收到的信用部分。 如果涉及多个潜在客户，则可能只是一个零头。</td> 
  </tr> 
  <tr> 
   <td>赢得的机会</td> 
   <td>为影响赢得的机会而收到的计划的信用部分。 如果涉及多个潜在客户，则可能只是一个零头。</td> 
  </tr> 
  <tr> 
   <td>已创建管道</td> 
   <td>为影响机会的创造而收到的方案的信用部分（以货币价值计）。 如果涉及多个潜在客户，则可能只是一个零头。</td> 
  </tr> 
  <tr> 
   <td>管道已创建 — 仍打开</td> 
   <td>为影响当前开放机会的创造而收到的方案的信用部分（货币价值）。 如果涉及多个潜在客户，则可能只是一个零头。</td> 
  </tr> 
  <tr> 
   <td>预期收入</td> 
   <td>为影响机会的创造而收到的方案的信用部分（以货币价值计）。 预期收入是机会概率乘以机会值。 如果涉及多个潜在客户，则可能只是一个零头。</td> 
  </tr> 
  <tr> 
   <td>投资收入</td> 
   <td>这是为影响赢得的机会而收到的方案的信用部分（货币价值）与方案成本之比。</td> 
  </tr> 
  <tr> 
   <td>收入赢得</td> 
   <td>为影响赢得的机会而收到的计划的信用部分（以货币价值计）。 如果涉及多个潜在客户，则可能只是一个零头。</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT)=首次联系归因，用于衡量潜在客户获取情况；(MT)=多接触归因，用于衡量潜在客户成功与否_

下面是一种方案，描述当存在两个生成潜在客户的程序，但这些潜在客户从同一帐户中导致一个Opportunity时，如何计算Opportunity Units。

**计划1**

* 生成一个潜在客户：潜在客户1
* 潜在客户1来自帐户1

**方案2**

* 生成另一个潜在客户：商机2
* 潜在客户2也来自帐户1

**帐户1**

* 生成一个机会：机会1

Marketo会适当地提供信用，而不会重复计算各个项目中的机会。 因此，在本例中，每个计划都接收0.5个机会单位。 也就是说，每个Program都收到所生成Opportunity的一半信用。 此外，与Opportunity关联的收入的一半被分配给每个Program。

## 与杂项方案有关的措施 {#miscellaneous-program-related-measures}

现有的其他措施反映了该方案的总体业绩。

<table> 
 <tbody> 
  <tr> 
   <th>归因度量 — 与项目相关</th> 
   <th>描述</th> 
  </tr> 
  <tr> 
   <td>与计划关联的机会数量</td> 
   <td><p>已将任何类型的归因点数分配给某个项目的Opportunity总数。 机会可能受一个或多个线索以及一个或多个项目的影响。</p></td> 
  </tr> 
  <tr> 
   <td>每个封闭机会的平均成功次数</td> 
   <td>在机会结束之前，计划成功的平均次数。 <br></td> 
  </tr> 
  <tr> 
   <td>每个机会创建的平均成功次数</td> 
   <td>在创建Opportunity之前， Programs成功的平均次数。</td> 
  </tr> 
  <tr> 
   <td>新名称</td> 
   <td>计划获得的新名称，即新潜在客户的总数。</td> 
  </tr> 
  <tr> 
   <td>计划成本</td> 
   <td>方案费用总额。</td> 
  </tr> 
  <tr> 
   <td>成功（总计）</td> 
   <td>成功的方案成员总数。</td> 
  </tr> 
 </tbody> 
</table>

## 计划机会分析Dimension（黄色圆点） {#program-opportunity-analysis-dimensions-yellow-dots}

虽然测量（蓝点）是计算的，并且需要一些思考和说明才能使用，但尺寸（黄色点）是描述性的。 以下是可用的维度。

<table> 
 <tbody> 
  <tr> 
   <th>类别</th> 
   <th>显示标签</th> 
  </tr> 
  <tr> 
   <td>机会属性</td> 
   <td>机会已结束<br>机会名称*<br>机会所有者名称<br>机会阶段<br>机会类型</td> 
  </tr> 
  <tr> 
   <td>机会时间范围</td> 
   <td>销售机会已结束年/季/月<br>业务机会创建年/季/月</td> 
  </tr> 
  <tr> 
   <td>程序属性</td> 
   <td>节目渠道<br>项目名称</td> 
  </tr> 
  <tr> 
   <td>计划成本时间范围</td> 
   <td>成本年/季/月</td> 
  </tr> 
 </tbody> 
</table>

*&#42;将任何类型的归因点数分配给某个项目的所有Opportunity。 机会可能受一个或多个线索以及一个或多个项目的影响。*

>[!MORELIKETHIS]
>
>[创建收入浏览器报表](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
