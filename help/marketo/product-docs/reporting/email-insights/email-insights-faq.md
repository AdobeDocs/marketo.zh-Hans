---
unique-page-id: 10100257
description: 电子邮件分析常见问题解答 — Marketo文档 — 产品文档
title: 电子邮件分析常见问题解答
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 电子邮件分析常见问题解答 {#email-insights-faq}

## 包含[!UICONTROL Email Insights]的比率指标与其他Marketo电子邮件报表之间是否有任何差异？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

可以。[!UICONTROL Email Insights]将参与度量与计算参与度量比率（打开率、点击打开率、取消订阅率）时发送的同一电子邮件的相应投放度量相关联。 例如，在[!UICONTROL Email Insights]中，当查看包含点击率每日细分的时间系列图表时，我们现在会根据相应的投放量度显示打开/点击/取消订阅事件的真实相关比率。 这与Revenue Explorer中的行为形成对比，后者只是将所有内容汇总起来。 [!UICONTROL Email Insights]提供了更准确的参与率视图。

## 为什么[!UICONTROL Email Insights]仅支持10个自定义维度？ {#why-does-email-insights-only-support-custom-dimensions}

对于许多用例，通过10个额外的自定义维度扩展默认系统维度已经足够，并且包括基于分段或程序标记的自定义维度。 将来，我们计划允许客户增加允许的自定义维度的数量。

## 为什么在分配自定义维度版块后无法重用这些版块？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

一旦分配了给定的自定义Dimension插槽，重新映射它将会导致以前的数据在与新含义混合时产生错误。 因此，自定义Dimension插槽可能无法重复使用。 此行为与其他量度分析工具(例如Google Analytics)的行为一致。

## [!UICONTROL Email Insights]是否支持Marketo Sales Insight电子邮件？ {#does-email-insights-support-marketo-sales-insight-emails}

可以。通过Marketo销售分析发送的所有电子邮件都包含在[!UICONTROL Email Insights]中。

## [!UICONTROL Email Insights]是否支持操作电子邮件？ {#does-email-insights-support-operational-emails}

可以。默认情况下，查看和查询会隐藏操作电子邮件。 但是，您可以在“个人设置”面板下更改此设置。

## [!UICONTROL Email Insights]是否捕获定期计划或重新运行Smart Campaign电子邮件流程步骤？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

“是”和“否”。 在[!UICONTROL Email Insights]的初始版本中，将为任何定期计划或重新运行的Smart Campaign捕获和访问所有电子邮件事件。 但是，您将无法区分该Smart Campaign的不同运行。 我们将在下一个版本中添加支持，以捕获Open、Click和Unsubscribe事件的Smart Campaign运行信息，以便区分。

## 为什么在按设备类型或设备操作系统进行过滤时，许多量度都显示为零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了点击打开率、打开次数、点击次数和取消订阅之外，所有其他受支持的量度都是交付事件或从交付事件派生的比率。 由于设备类型和设备操作系统仅适用于参与量度，因此我们根本没有可显示的信息。 例如，在按设备类型=移动设备进行筛选时，询问投放率是未定义的查询，因为Marketo不会收到基础投放和已发送事件的任何参与量度。 我们正在探索从参与量度中应用设备类型和设备操作系统的方法，以匹配包含参与和交付量度的比率。

## 当某些电子邮件客户端阻止图像时，[!UICONTROL Email Insights]做什么？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一个常见的行业问题是，越来越多的电子邮件客户端默认关闭了图像。 加载图像是记录打开次数的基础。 用户完全有可能收到一封电子邮件，其中图像被阻止，但文本和链接完全可读。 如果用户遇到这种情况，点击了该电子邮件中的链接，您最终可能会遇到点击事件场景，但不会收到针对该电子邮件的相应的“打开”事件。 Marketo电子邮件分析将自动生成任何缺失的事件。 该逻辑与Marketo为电子邮件性能报表以及Revenue Explorer中的电子邮件分析区域执行此操作的方式相同。
