---
unique-page-id: 12979858
description: 性能分析常见问题解答 — Marketo文档 — 产品文档
title: 性能分析常见问题解答
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# 性能分析常见问题解答 {#performance-insights-faq}

## “参与”选项卡中“成功”的定义是什么？ {#what-is-the-definition-of-success-in-the-engagement-tab}

成功是衡量Marketo中是否存在有意义的互动的一个指标。 项目的目的是创建与人员或潜在客户的有意义的交互。 当人员达到达到达到该目标的状态时，将标记成功。 它可以参加网络研讨会、单击电子邮件中的链接或填写Web表单。 成功情况因项目渠道而异。

>[!NOTE]
>
>网络研讨会计划可有多个状态，如：受邀、已注册和已参加。 “已邀请”或“已注册”不是有意义的交互，因为人们实际上并不观看网络研讨会。 在这种情况下，已出席被视为成功。

## MPI是否可与任何CRM配合使用？ {#will-mpi-work-with-any-crm}

是. 从技术上讲，MPI不会直接与CRM交互以进行数据同步。 MPI利用存储在Marketo AnalyticsData warehouse中的数据。 由于CRM同步发生在商机管理应用程序中，因此Marketo支持的与商机管理应用程序集成的CRM将正确显示数据。 但是，需要将CRM opportunity字段正确映射到Marketo opportunity字段。

## 我没有任何其他Marketing Analytics产品（ARB、RCE、RCA、项目分析）。 MPI会为我工作吗？ {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI是Lead Management应用程序的独立附加产品。 它不需要使用任何其他分析产品。

## RCA也向我显示程序性能数据。 MPI和RCA中显示的数据是否存在差异？ {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

否. MPI从与RCA相同的data warehouse获取数据。 因此，您将不会看到两者之间的任何数据差异。 RCA允许您动态创建自己的报告。 MPI让您能够访问易于理解的可视化仪表板。

## 我不想在MPI中显示我的某些程序（例如，Operational）。 如何控制特定程序的可见性？ {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

通过将程序的Analytics行为设置为“可操作”，您可以控制程序的可见性。 这将导致从分析计算中排除该程序。

>[!NOTE]
>
>了解有关设置分析行为的更多信息 [此处](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## 我正在为新产品发布运行多渠道营销活动。 如何在一个位置跨所有不同渠道查看此营销活动的效果？ {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

我们建议，对于此类营销策划中的项目，请使用项目标记。 项目标记会自动同步到MPI，您可以在所有MPI功能板中过滤这些标记，以查看您的多渠道营销活动效果。

## 如果没有RCA，我是否可以访问归因设置？ {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

如果您有MPI，则无论您是否拥有RCA，都可以访问归因设置。

## 当我登录并告知归因设置不正确时，会在MPI中收到警报。 有什么问题吗？ {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI会计算您的所有机会是否都包含在Analytics中。 否则，系统将提示您考虑更改归因设置（显式、隐式、混合）以包含更多机会。

您也可能由于项目中缺少项目成本而缺少机会。 请检查程序的Analytics行为。 它们可以是：

1. 默认 — 默认行为是，只有在至少有一个期间成本（即使分配了零美元）时，MPI中才会包含程序。

1. 包含 — 此选项将确保MPI中的程序可用，无论您是否包括期间成本。

1. [可操作](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs)  — 此选项导致程序无法在MPI中显示。

>[!NOTE]
>
>期间成本 **具有** 要在参与仪表板中为成功和新名称报告进行设置。 此仪表板利用期间成本数据来汇总成功和新名称。 如果未设置期间成本，则无论上述Analytics行为设置如何，参与度仪表板都将无法正确报告。

## 为什么我错过了在MPI中的一些机会？ {#why-am-i-missing-some-opportunities-in-mpi}

您可能错过MPI销售机会的两个关键原因是：

1. 归因设置设为“显式”，但机会未分配联系人角色
1. 期间成本不包括在您的计划中

MPI会计算您的所有机会是否都包含在Analytics中。 否则，系统将提示您考虑更改归因设置（显式、隐式、混合）以包含更多机会。

您也可能由于项目中缺少项目成本而缺少机会。 系统会发出警告，但不会向您指出哪些项目缺少成本。 请检查您的项目设置以包括成本，以确保您的所有项目和机会都包含在MPI中。

## 为什么在Engagement仪表板上看不到Custom Fields 、 Opportunity Type和ABM过滤器？ {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

自定义字段、业务机会类型和ABM筛选器都是与业务机会相关的属性。 Engagement仪表板允许您衡量参与和潜在客户获取，无论它们是否与opportunity关联。 由于Engagement仪表板未考虑opportunity ，因此Custom Fields 、 Opportunity Type和ABM筛选器不适用。

## 我想使用自定义Salesforce Opportunity字段而不是标准Salesforce Opportunity Amount字段来报告收入。 MPI允许我执行此操作吗？ {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

是. [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 能够将Marketo的Opportunity Amount字段重新映射到自定义Salesforce Opportunity字段，只要该字段类型为货币。 由于MPI指向Marketo Opportunity amount字段，因此MPI可以使用重新映射的自定义Salesforce字段中的数据。

>[!NOTE]
>
>重新映射后，MPI将显示以后的数据。 历史金额不会改变。

## 如果不利用机会，还可以使用MPI吗？ {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI旨在让您从漏斗顶部开始衡量项目绩效，直至收入影响。 如果不利用机会，您仍然能够：

* 查看您的培养计划的表现以吸引受众参与。
* 查看潜在客户获取计划的性能。
* 通过项目标记查看多渠道营销活动的效果。
* 查看过去12个月的受众参与趋势。
* 在PowerPoint中保存并导出性能数据。

## 我能否衡量MPI中基于帐户的策略是否成功？ {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

是. MPI与 [MARKETO TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) 将ABM帐户列表无缝地拉入MPI。 您可以使用“ABM帐户列表”筛选器来选择所需的ABM列表以过滤数据。

## 购买MPI时是否可以立即使用归因？ {#is-attribution-instantly-available-when-i-purchase-mpi}

我们的客户在购买MPI时，可以使用Marketo归因功能。 但是， [正确设置](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) 是确保机会和程序数据正确地流入MPI所必需的。

## 我该怎么做才能设置归因？ {#what-do-i-have-to-do-to-set-up-attribution}

1. 机会设置

   1. 确保机会与CRM同步
   1. 如果“归因”设置设为“明确”，请确保填充机会上的联系人角色
   1. 我们建议将归因设置更改为混合
   1. 项目设置

      1. 将项目成本包括在您的项目中
      1. 查看Analytics行为以指示是否应在Analytics中包含程序
      1. 为您拥有的每个渠道设置成功标准
      1. 将人员绑定到计划

         1. 确保已为数据库中的每个人设置客户获取计划和客户获取日期，以便首次联系归因正常工作。
         1. 确保程序为数据库中的人员设置成功状态

>[!TIP]
>
>有关所需的所有设置步骤的详情，请参见 [本文](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## MPI与Program Analyzer之间有何区别？ {#whats-the-difference-between-mpi-and-the-program-analyzer}

程序分析器允许您最多四个指标对程序进行比较。 MPI允许您分析渠道和项目对所选量度（如成功、创造的新机会等）的贡献。 它还允许您根据所选的特定量度查看12个月的渠道趋势。

## MPI和高级Report Builder之间有何区别？ {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

高级Report Builder（有时称为RCE）专为自助（或临时）报表而设计，通常由营销运营完成。 MPI旨在为营销领导和营销人员提供对性能分析的一次性访问。 需要最少的设置。

## 贡献日期筛选器中的“上一年”选项发生了什么情况？ {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

我们暂时删除了“上一年”选择。 您仍然可以选择使用自定义日期范围选项查看整年的性能数据。
