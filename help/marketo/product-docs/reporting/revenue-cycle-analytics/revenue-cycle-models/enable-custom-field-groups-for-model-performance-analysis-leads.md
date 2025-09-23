---
unique-page-id: 3571890
description: 为模型性能分析（潜在客户）启用自定义字段组 — Marketo文档 — 产品文档
title: 为模型绩效分析（潜在客户）启用自定义字段组
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 6%

---

# 为模型绩效分析（潜在客户）启用自定义字段组 {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>通过Marketo中的字段管理器将标准字段或自定义字段分类为要报告的组。 有关详细信息，请参阅[通过字段管理器创建自定义字段组](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md)。

<table>
 <tbody>
  <tr>
   <td colspan="3" rowspan="1"><p align="center"><strong>启用自定义字段组如何影响Revenue Cycle Explorer中的多个分析区域？</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>当……发生什么情况？</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>它如何影响<span class="uicontrol">模型性能分析（潜在客户）</span>区域</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>它如何影响潜在客户分析、营销活动分析和机会分析领域</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>当您启用与标准潜在客户或公司字段关联的自定义字段组时，会发生什么情况？</strong></p></td>
   <td colspan="1" rowspan="1"><p>自定义字段组已在<span class="uicontrol">模型性能分析（潜在客户）</span>区域启用报告</p></td>
   <td colspan="1" rowspan="1"><p>无影响</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>当您启用与自定义人员或公司字段关联的自定义字段组时，会发生什么情况？</strong></p></td>
   <td colspan="1" rowspan="1"><p>自定义字段组已在<span class="uicontrol">模型性能分析（潜在客户）</span>区域启用报告</p></td>
   <td colspan="1" rowspan="1"><p>自定义字段本身可用于在Lead Analysis 、 Campaign Analysis和Opportunity Analysis区域报告。</p><p><strong>注意：</strong>这些分析区域不支持自定义字段组，因此组关联不会显示在收入周期资源管理器中 — <em>仅</em>自定义字段。</p></td>
  </tr>
 </tbody>
</table>

按照以下步骤在[!UICONTROL Model Performance Analysis (Leads)]区域中启用用于报告的自定义字段组。

1. 单击 **[!UICONTROL Admin]**。

   ![](assets/one-1.png)

1. 单击 **[!UICONTROL Revenue Cycle Analytics]**。

   ![](assets/two-1.png)

1. 单击空字段组旁边的&#x200B;**[!UICONTROL None]**。 如果已启用三个字段组并想要进行编辑，请单击要修改的字段组的名称。

   ![](assets/three.png)

1. 单击&#x200B;**[!UICONTROL Field]**&#x200B;下拉列表并选择您想要的。

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >此示例为标准字段(State)启用了自定义字段组。 因此，只有[!UICONTROL Model Performance Analysis (Leads)]区域受到影响。 如果已为自定义人员或公司字段启用自定义字段组，则启用的组将显示在“同步摘要”选项卡的[!UICONTROL Model Performance Analysis (Leads)]部分中，并且商机、营销活动和机会分析的自定义字段计数将增加1。

1. 单击 **[!UICONTROL Save]**。

   ![](assets/five-1.png)
