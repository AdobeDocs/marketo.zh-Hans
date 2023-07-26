---
unique-page-id: 3571890
description: 为模型性能分析（潜在客户）启用自定义字段组 — Marketo文档 — 产品文档
title: 为模型性能分析（潜在客户）启用自定义字段组
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 为模型性能分析（潜在客户）启用自定义字段组 {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>通过Marketo中的字段管理器将标准字段或自定义字段分类为要报告的组。 有关详细信息，请参阅 [通过字段管理器创建自定义字段组](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>启用自定义字段组如何影响Revenue Cycle Explorer中的多个分析区域？</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>当……发生什么情况？</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>它如何影响模型性能分析（潜在客户）区域</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>它如何影响潜在客户分析、营销活动分析和机会分析领域</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>当您启用与标准潜在客户或公司字段关联的自定义字段组时，会发生什么情况？</strong></p></td> 
   <td colspan="1" rowspan="1"><p>自定义字段组已为“模型性能分析（潜在客户）”区域中的报表启用</p></td> 
   <td colspan="1" rowspan="1"><p>无影响</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>当您启用与自定义人员或公司字段关联的自定义字段组时，会发生什么情况？</strong></p></td> 
   <td colspan="1" rowspan="1"><p>自定义字段组已为“模型性能分析（潜在客户）”区域中的报表启用</p></td> 
   <td colspan="1" rowspan="1"><p>自定义字段本身可用于在Lead Analysis 、 Campaign Analysis和Opportunity Analysis区域报告。</p><p><strong>注意：</strong> 这些分析区域不支持自定义字段组，因此组关联不显示在Revenue Cycle Explorer—<em>仅限</em> 自定义字段。</p></td> 
  </tr> 
 </tbody> 
</table>

按照以下步骤启用自定义字段组，以便在模型性能分析（潜在客户）区域进行报告。

1. 单击 **管理员**.

   ![](assets/one-1.png)

1. 单击 **收入周期分析**.

   ![](assets/two-1.png)

1. 单击 **无** 空字段组旁边。 如果已启用三个字段组并想要进行编辑，请单击要修改的字段组的名称。

   ![](assets/three.png)

1. 单击 **字段** 下拉列表并选择您想要的。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >此示例为标准字段(State)启用了自定义字段组。 因此，仅模型性能分析(Leads)区域受到影响。 如果已为自定义人员或公司字段启用了自定义字段组，则已启用的组将显示在“同步摘要”选项卡的“模型性能分析（潜在客户）”部分中，并且潜在客户、促销活动和机会分析的自定义字段计数将增加1。

1. 单击 **保存**.

   ![](assets/five-1.png)
