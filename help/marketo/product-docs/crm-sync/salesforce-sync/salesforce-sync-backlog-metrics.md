---
description: Salesforce同步积压量度 — Marketo文档 — 产品文档
title: Salesforce同步积压量度
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 1cc876285f8d7ac7a21a763dd65da34341341a0e
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Salesforce同步积压量度  {#salesforce-sync-backlog-metrics}

同步积压表示从Salesforce到Marketo Engage的待同步记录，反之亦然。 确保积压问题得到控制将实现顺利和及时的同步。

>[!NOTE]
>
>积压工作包括两端的待处理同步后更新数，而不是同步流程步骤(如[将人员同步到SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}或[将人员同步到Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}流程步骤)执行的数量。

## 如何访问 {#how-to-access}

1. 在Marketo Engage中，转到&#x200B;**管理员**&#x200B;区域。

   屏幕快照

1. 选择&#x200B;**Salesforce**。

   屏幕快照

## 同步积压事项趋势 {#sync-backlog-trend}

积压趋势反映过去5天记录的积压更改。 积压以4小时间隔显示，间隔为5天。 因此，该图表将每天显示6个间隔，乘以5天，这等于30个间隔。

在x轴上以特定的4小时间隔观察积压。 此值适用于正在同步的所有对象。 这是Salesforce和Marketo Engage中等待同步的积压工作总数。

屏幕快照

## 同步吞吐量和积压 {#sync-throughput-and-backlog}

统计信息反映过去24小时内同步下每种对象类型的吞吐量和积压状态。 对象类型包括同步下的所有对象，包括：潜在客户、联系人、帐户、机会、促销活动、用户和自定义对象。 吞吐量统计信息每15分钟自动刷新一次，但您可以使用刷新图标手动刷新。 每小时获取积压一次。

>[!NOTE]
>
>统计信息是按滚动日期更新的，而不是按日历日更新。

屏幕快照

<table><thead>
  <tr>
    <th>字段</th>
    <th>描述</th>
  </tr></thead>
<tbody>
  <tr>
    <td>同步的最大记录数/小时</td>
    <td>对象类型在过去24小时内观察到的每小时同步的最大记录数（最大吞吐量）。 24小时期间会随时间滚动，而不是随着日历日滚动。</td>
  </tr>
  <tr>
    <td>同步的最小记录数/小时</td>
    <td>对象类型在过去24小时内每小时同步的最小记录数（最小吞吐量）。 24小时期间会随时间滚动，而不是随着日历日滚动。</td>
  </tr>
  <tr>
    <td>平均同步记录数/小时</td>
    <td>对象类型在过去24小时内每小时同步的平均记录数（最小吞吐量）。 24小时期间会随时间滚动，而不是随着日历日滚动。 此值计算为过去24小时内同步的总记录数。</td>
  </tr>
  <tr>
    <td>同步积压</td>
    <td>对象类型的待同步记录的积压。 它是两个方向(从Salesforce到Marketo Engage，反之亦然)的待同步积压的总和。 来自Salesforce的积压事项是通过Salesforce的API调用获得的，来自Marketo Engage的积压事项是使用从变更数据日志获得的统计数据计算的。 每小时计算一次。 此表中的下两个字段分别通知上次计算积压的时间，以及下一个计算计划。</td>
  </tr>
  <tr>
    <td>估计积压（时间）</td>
    <td>按对象类型同步积压所需的估计时间。 计算为“同步积压/每小时同步的平均记录数”。</td>
  </tr>
  <tr>
    <td>上次获取的积压工作</td>
    <td>上次积压计算的时间。</td>
  </tr>
  <tr>
    <td>积压下一个获取</td>
    <td>下次积压计算的时间。</td>
  </tr>
  <tr>
    <td>积压状态</td>
    <td>这会显示积压在过去6小时内是否有所增加。 如果当前积压大于6小时前记录的积压，则推断为“正在增长”。 否则，将显示为“正常”。 这是为了显示同步吞吐量是否正在赶上积压工作。</td>
  </tr>
</tbody></table>

## 导致同步积压的原因 {#what-causes-sync-backlogs}

无论是在Marketo Engage端还是CRM端进行更新，都会触发要重新同步的记录，通过向CRM的常规Marketo Engage周期更新另一端的信息。 每当对Salesforce上的记录进行更新时，都会生成一个系统修改时间戳，称为“SysModStamp”。 此队列将更改排入同步队列。

当进行大量更新（例如更改字段值）时，许多记录会更改，从而导致出现新的SysModStamps。 然后，大量人员记录更新需要在Marketo Engage和您的CRM之间重新同步，有时会创建临时积压。

## 管理同步积压的最佳实践 {#best-practices}

**同步下的字段**：确保同步下的字段仅为需要同步的字段。 更改字段会增加同步积压，而优先级较低的字段可能会停止或减慢正在同步的更重要的字段。 联系[Marketo Engage支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}以移除同步下的字段。

**敏感字段**：某些字段容易频繁更新（例如，可能会发生货币更改的货币字段）。 检查是否需要同步这些字段，或者是否需要以不同的方式设计字段。

**自定义对象**：定期查看正在同步的自定义对象，并删除不再需要同步的任何自定义对象。

**活动**：检查同步下是否存在可以从同步中删除的任何活动。

**在非关键时间安排批量更新**：查看您的数据同步模式以识别非关键时间段。 查看是否可以在这些非关键期间计划批量更新。

如果您正在遵循上述所有最佳实践，但仍遇到大量积压问题，请联系[Marketo Engage支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。
