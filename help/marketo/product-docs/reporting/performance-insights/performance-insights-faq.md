---
unique-page-id: 12979858
description: 性能分析常见问题解答 — 营销文档 — 产品文档
title: 性能洞察常见问题解答
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---


# 性能分析常见问题解答{#performance-insights-faq}

## “参与”选项卡中“成功”的定义是什么？{#what-is-the-definition-of-success-in-the-engagement-tab}

成功是衡量Marketo中有意义互动的指标。 项目的目的是与个人或潜在客户创建有意义的交互。 当某人达到该目标的状态时，会标记成功。 它可以参加网络研讨会，单击电子邮件中的链接，或填写Web表单。 成功情况因项目渠道而异。

>[!NOTE]
>
>在网络研讨会项目中，可能有多种状态，例如：已邀请、已注册和已出席。 “已邀请”或“已注册”并非有意义的交互，因为人们实际上不会观看网络研讨会。 在这种情况下，已出席被视为成功。

## MPI是否可以与任何CRM一起使用？{#will-mpi-work-with-any-crm}

是的。 技术上，MPI不直接与CRM进行数据同步交互。 MPI利用存储在Marketo AnalyticsData warehouse中的数据。 由于CRM同步发生在Lead Management应用程序中，因此任何与Lead Management应用程序集成的Marketo支持的CRM都将正确显示数据。 但是， CRM业务机会字段确实需要正确映射到Marketo业务机会字段。

## 我没有任何其他Marketing Analytics产品(ARB、RCE、RCA、项目分析)。 MPI能为我效劳吗？{#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI是Lead Management应用程序的独立加载项。 它不需要使用任何其他分析产品。

## RCA还向我展示了项目性能数据。 MPI和RCA中显示的数据之间是否有差异？{#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

不。 MPI从与RCA相同的data warehouse中源数据。 因此，您不会看到两者之间的任何数据差异。 RCA允许您飞快创建自己的报告。 MPI使您能访问易于理解的可视仪表板。

## 我不希望我的某些项目（例如操作）在MPI中显示。 如何控制特定项目的可见性？{#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

您可以将项目的“分析”行为设置为“操作”，从而控制项目的可见性。 这将导致项目从分析计算中排除。

>[!NOTE]
>
>了解有关设置分析行为[的更多信息，请访问](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md)。

## 我正在为新产品发布运行多渠道活动。 如何在一个位置视图此活动在所有不同渠道中的性能？{#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

我们建议，对于此类活动的项目部分，您应使用项目标记。 项目标签会自动同步到MPI，您可以在所有MPI仪表板中过滤它们以视图多渠道活动性能。

## 如果没有RCA，我是否将有权访问归因设置？{#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

如果您有MPI，则无论您是否有RCA，您都可以访问归因设置。

## 我登录后会在MPI中收到警报，告知我的归因设置不正确。 怎么了？{#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI会计算是否您的所有机会都包含在分析中。 否则，系统将提示您考虑更改您的属性设置（显式、隐式、混合）以包含更多机会。

由于项目成本在您的项目中缺失，您可能也缺少机会。 请查看您项目的Analytics行为。 它们可以是：

1. 默认 — 默认行为是，只有至少存在一个期间成本（即使分配了零美元）时，项目才会包含在MPI中。

1. 包含 — 此选项将确保MPI中提供项目，而不管您是否包含期间成本。

1. [操作](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs)  — 此选项导致项目在MPI中不显示。

>[!NOTE]
>
>期间成本&#x200B;**在“参与”仪表板中为“成功和新名称”报告设置**。 此仪表板利用期间成本数据来聚合成功案例和新名称。 如果未设置“期间成本”，则无论上述Analytics行为设置如何，参与仪表板都将无法正确报告。

## 为什么我在MPI中缺少一些机会？{#why-am-i-missing-some-opportunities-in-mpi}

您在MPI中可能缺少机会的两个主要原因是：

1. 归因设置设置为“显式”，但Opportunity未分配“联系角色”
1. 期间成本不包括在您的项目中

MPI会计算是否您的所有机会都包含在分析中。 否则，系统将提示您考虑更改您的属性设置（显式、隐式、混合）以包含更多机会。

由于项目成本在您的项目中缺失，您可能也缺少机会。 警报会发出，但不会指出哪些项目缺少成本。 请检查您的项目设置以包括成本，以确保MPI中包含您的所有项目和机会。

## 为什么在“参与”仪表板中看不到“自定义字段”、“机会类型”和“ABM过滤器”？{#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

自定义字段、业务机会类型和ABM过滤器都是与业务机会相关的属性。 参与仪表板允许您衡量您的参与度和潜在客户赢取情况，无论他们是否与某个机会关联。 由于“参与”仪表板未考虑机会，因此“自定义字段”、“机会类型”和“ABM过滤器”不适用。

## 我要使用自定义Salesforce Opportunity字段来报告收入，而不是标准Salesforce Opportunity Amount字段。 MPI会允许我这样做吗？{#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

是的。 [只要字](https://nation.marketo.com/t5/Support/ct-p/Support) 段类型是货币， Marketo Supportion就可以将Marketo的Opportunity Amount字段重新映射到自定义Salesforce Opportunity字段。由于MPI指向Marketo Opportunity金额字段，因此MPI可以使用重新映射的自定义Salesforce字段中的数据。

>[!NOTE]
>
>重新映射后，MPI将显示数据的未来。 历史数量不会改变。

## 如果我不利用机会，我还能使用MPI吗？{#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI旨在允许您从漏斗顶部到收入影响的项目性能。 如果您不使用机会，您仍能够：

* 视图性能，让您的培养项目参与受众。
* 视图您的潜在客户赢取项目的表现。
* 通过视图标签实现多渠道活动的项目性能。
* 查看过去12个月的受众参与趋势。
* 在PowerPoint中保存和导出性能数据。

## 我能否衡量MPI中基于帐户的策略的成功程度？{#can-i-measure-the-success-of-account-based-strategies-in-mpi}

是的。 MPI与[Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview)集成，可将ABM帐户列表无缝地引入MPI。 您可以使用ABM帐户列表过滤器来选择所需的ABM列表以过滤数据。

## 我购买MPI时是否即时可用归因？{#is-attribution-instantly-available-when-i-purchase-mpi}

客户购买MPI时，可以使用Marketo Attribution功能。 但是，需要[正确的设置](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md)才能确保机会和项目数据正确流入MPI。

## 要设置归因，我必须做什么？{#what-do-i-have-to-do-to-set-up-attribution}

1. 机会设置

   1. 确保机会与您的CRM同步
   1. 如果您的归因设置设置为“显式”，请确保填充了Opportunity上的联系人角色
   1. 我们建议将“属性”设置更改为“混合”
   1. 项目设置

      1. 将项目成本纳入项目
      1. 查看分析行为，以指示是否应将项目包含在分析中
      1. 设置每个渠道的成功标准
      1. 将人员与项目

         1. 确保已为数据库中的每个人设置“客户获取项目”和“客户获取日期”，以使“首次联系归因”正常工作。
         1. 确保您的项目正在为数据库中的人员设置成功状态

>[!TIP]
>
>本文[中详细介绍了所需的所有设置步骤。](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md)

## MPI和项目分析器之间有何区别？{#whats-the-difference-between-mpi-and-the-program-analyzer}

项目分析器允许您对多达四个度量的项目进行比较。 MPI允许您分析渠道和项目对选定量度的贡献，如“成功”、“新创造的机会”等。 它还允许您根据您选择的一个特定量度视图12个月渠道趋势。

## MPI与高级Report Builder有何区别？{#whats-the-difference-between-mpi-and-the-advanced-report-builder}

高级Report Builder（有时称为RCE）专为自助（或临时）报告而设计，通常由营销运营部门完成。 MPI旨在让营销领导者和营销人员只需单击一下即可访问性能分析。 需要的设置最少。

## 贡献的日期过滤器中的“上一年”选项发生了什么情况？{#what-happened-to-the-previous-year-option-in-contributions-date-filter}

我们暂时删除了“上一年”选项。 您仍可以选择使用“自定义日期范围”选项来查看整年的性能数据。
