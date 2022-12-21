---
unique-page-id: 12979858
description: 性能分析常见问题解答 — Marketo文档 — 产品文档
title: 性能分析常见问题解答
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# 性能分析常见问题解答 {#performance-insights-faq}

## “参与度”选项卡中“成功”的定义是什么？ {#what-is-the-definition-of-success-in-the-engagement-tab}

在Marketo，成功是有意义互动的衡量标准。 项目的目的是与人员或潜在客户进行有意义的互动。 当人员达到达到该目标的状态时，即表示成功。 它可以参加网络研讨会，单击电子邮件中的链接，或填写Web表单。 成功情况因节目渠道而异。

>[!NOTE]
>
>在网络研讨会计划中，可以有多种状态，例如：已邀请、已注册并已出席。 “已邀请”或“已注册”并不是有意义的交互，因为用户实际上不会观看网络研讨会。 在这种情况下，已参加被视为成功。

## MPI是否可与任何CRM配合使用？ {#will-mpi-work-with-any-crm}

是. 从技术上讲，MPI不会直接与CRM进行交互以进行数据同步。 MPI利用存储在Marketo AnalyticsData warehouse中的数据。 由于CRM同步是在潜在客户管理应用程序中进行的，因此任何与潜在客户管理应用程序集成在Marketo支持的CRM都将正确显示数据。 但是， CRM机会字段确实需要正确映射到Marketo机会字段。

## 我没有任何其他Marketing Analytics产品(ARB、RCE、RCA、Program Analysis)。 MPI能为我效劳吗？ {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI是“潜在客户管理”应用程序的独立附加组件。 它不需要使用任何其他分析产品。

## RCA还显示了程序性能数据。 MPI和RCA中显示的数据是否有差异？ {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

否. MPI从与RCA相同的data warehouse中源数据。 因此，您将看不到两者之间的任何数据差异。 RCA允许您即时创建自己的报告。 MPI让您能够访问易于理解的可视化功能板。

## 我不希望我的某些程序（如操作）在MPI中显示。 如何控制特定程序的可见性？ {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

您可以将项目的Analytics行为设置为“操作”，从而控制项目的可见性。 这将导致程序被排除在分析计算之外。

>[!NOTE]
>
>了解有关设置分析行为的更多信息 [此处](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## 我正在为新产品发布运行多渠道营销活动。 如何在一个位置查看此营销活动在所有不同渠道中的效果？ {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

我们建议，对于此类营销策划的项目部分，您应使用项目标记。 程序标记会自动同步到MPI，您可以在所有MPI功能板中过滤它们，以查看多渠道营销活动的效果。

## 如果我没有RCA，我是否有权访问归因设置？ {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

无论您是否具有RCA，如果您具有MPI，则可以访问归因设置。

## 当我登录时，在MPI中会收到一则警报，告知我的归因设置不正确。 怎么了？ {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI计算是否将您的所有机会都包含在Analytics中。 如果没有，系统将提示您考虑更改归因设置（显式、隐式、混合）以包含更多商机。

您可能还因程序成本在程序中缺失而缺少机会。 请查看您程序的Analytics行为。 它们可以是：

1. 默认 — 默认行为是，只有在至少有一个期间成本（即使分配了零美元）时，程序才会包含在MPI中。

1. 包含 — 此选项将确保该程序在MPI中可用，无论您是否已包括期间成本。

1. [运行](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs)  — 此选项导致程序在MPI中不显示。

>[!NOTE]
>
>期间成本 **has** 要在参与度仪表板中为成功和新名称报表进行设置。 此功能板利用期间成本数据来汇总成功案例和新名称。 如果未设置期间成本，则无论上述Analytics行为设置如何，参与仪表板都将无法正确报告。

## 为什么我在MPI中缺少一些机会？ {#why-am-i-missing-some-opportunities-in-mpi}

MPI中可能缺少机会的两个关键原因是：

1. 归因设置设置为“明确”，但商机没有分配“联系人角色”
1. 期间成本未包含在您的项目中

MPI计算是否将您的所有机会都包含在Analytics中。 如果没有，系统将提示您考虑更改归因设置（显式、隐式、混合）以包含更多商机。

您可能还因程序成本在程序中缺失而缺少机会。 系统会发出警报，但不会指出哪些程序缺少成本。 请检查您的程序设置以包含成本，以确保MPI中包含您的所有程序和机会。

## 为什么“参与”仪表板上没有看到“自定义字段”、“机会类型”和“ABM过滤器”？ {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

自定义字段、机会类型和ABM过滤器都与机会相关。 “参与度”仪表板允许您衡量您的参与度和潜在客户获取，无论他们是否与某个机会关联。 由于参与仪表板未考虑机会，因此自定义字段、机会类型和ABM过滤器不适用。

## 我希望使用自定义Salesforce Opportunity字段来报告收入，而不是标准的Salesforce Opportunity Amount字段。 MPI会允许我这样做吗？ {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

是. [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 只要字段类型是货币，就能将Marketo的Opportunity Amount字段重新映射到自定义的Salesforce Opportunity字段。 由于MPI指向Marketo Opportunity金额字段，因此MPI可以使用重新映射的自定义Salesforce字段中的数据。

>[!NOTE]
>
>重新映射后，MPI将显示未来的数据。 历史数量不会改变。

## 如果我不利用机会，我还能使用MPI吗？ {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI旨在允许您从漏斗顶部到收入影响来测量程序性能。 如果您不使用机会，您仍然能够：

* 查看您针对受众参与的培养计划的效果。
* 查看潜在客户获取计划的性能。
* 通过项目标记查看多渠道营销活动的效果。
* 请参阅过去12个月的受众参与趋势。
* 在PowerPoint中保存和导出性能数据。

## 我能否在MPI中衡量基于帐户的策略是否成功？ {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

是. MPI与 [Marketo](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) 将ABM帐户列表无缝地纳入MPI。 您可以使用“ABM帐户列表”过滤器选择所需的ABM列表以过滤数据。

## 购买MPI时，归因是否会立即可用？ {#is-attribution-instantly-available-when-i-purchase-mpi}

客户购买MPI时，可以使用Marketo归因功能。 但是， [正确设置](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) 需要确保机会和程序数据正确地流入MPI。

## 设置归因时我必须执行哪些操作？ {#what-do-i-have-to-do-to-set-up-attribution}

1. 机会设置

   1. 确保商机与您的CRM同步
   1. 如果您的Attribution设置设置为Explicit，请确保填充了Opportunity中的联系角色
   1. 我们建议将归因设置更改为混合
   1. 程序设置

      1. 将计划成本包含在您的计划中
      1. 查看分析行为以指示是否应将某个程序包含在分析中
      1. 为您拥有的每个渠道设置成功标准
      1. 将人员与项目绑定

         1. 确保为数据库中的每个人设置了客户获取程序和客户获取日期，以便首次联系归因正常工作。
         1. 确保您的程序正在为数据库中的人员设置成功状态

>[!TIP]
>
>有关所需的所有设置步骤的详细信息，请参阅 [本文](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## MPI与程序分析器之间有何区别？ {#whats-the-difference-between-mpi-and-the-program-analyzer}

程序分析器允许您对最多四个度量的程序进行比较。 MPI允许您分析渠道和程序对所选量度的贡献，如成功、新机会创造等。 它还允许您根据您选择的一个特定量度查看12个月的渠道趋势。

## MPI与高级Report Builder之间有何区别？ {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

高级Report Builder（有时称为RCE）专为自助（或临时）报表而设计，通常由营销操作完成。 MPI旨在让营销领导和营销人员一键访问性能分析。 需要的设置最少。

## 贡献的日期过滤器中的“上一年”选项发生了什么情况？ {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

我们暂时删除了“上一年”选项。 您仍可以选择使用自定义日期范围选项来查看全年的性能数据。
