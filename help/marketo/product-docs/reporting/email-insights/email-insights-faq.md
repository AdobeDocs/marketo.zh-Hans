---
unique-page-id: 10100257
description: 电子邮件分析常见问题解答 — Marketo文档 — 产品文档
title: 电子邮件分析常见问题解答
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 电子邮件分析常见问题解答 {#email-insights-faq}

## 具有电子邮件分析的比率指标与其他Marketo电子邮件报表之间是否有任何差异？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

是. 电子邮件分析将参与量度与计算参与量度比率（打开率、点击打开率、取消订阅率）时发送的同一电子邮件的相应投放量度相关联。 例如，在电子邮件分析中，查看过去一周包含点击率每日细分的时间系列图表时，我们现在会根据相应的投放量度显示打开/点击/取消订阅事件的真实相关比率。 这与Revenue Explorer中的行为形成对比，后者只是将所有内容汇总起来。 电子邮件分析可更准确地查看参与率。

## 为什么电子邮件分析仅支持10个自定义Dimension？ {#why-does-email-insights-only-support-custom-dimensions}

对于许多用例，通过10个额外的自定义维度扩展默认系统维度已经足够，并且包括基于分段或程序标记的自定义维度。 将来，我们计划允许客户增加允许的自定义Dimension的数量。

## 为什么在分配自定义Dimension版块后无法重复使用这些版块？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

一旦分配了给定的自定义Dimension槽，重新映射它将会导致以前的数据在与新含义混合时产生错误。 因此，自定义Dimension槽不能重复使用。 此行为与其他量度分析工具(例如Google Analytics)的行为一致。

## 电子邮件分析是否支持Marketo销售分析电子邮件？ {#does-email-insights-support-marketo-sales-insight-emails}

是. 通过Marketo Sales Insights发送的所有电子邮件都包含在电子邮件分析中。

## 电子邮件分析是否支持操作电子邮件？ {#does-email-insights-support-operational-emails}

是. 默认情况下，查看和查询会隐藏操作电子邮件。 但是，您可以在“个人设置”面板下更改此设置。

## 电子邮件分析会捕获定期计划还是重新运行Smart Campaign电子邮件流程步骤？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

“是”和“否”。 在Email Insights的初始版本中，可捕获所有电子邮件事件并为任何定期计划或重新运行的Smart Campaign访问。 但是，您将无法区分该Smart Campaign的不同运行。 我们将在下一个版本中添加支持，以捕获Open、Click和Unsubscribe事件的Smart Campaign运行信息，以便区分。

## 为什么在按设备类型或设备操作系统进行过滤时，许多量度都显示为零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除了点击打开率、打开次数、点击次数和取消订阅之外，所有其他受支持的量度都是交付事件或从交付事件派生的比率。 由于设备类型和设备操作系统仅适用于参与量度，因此我们根本没有可显示的信息。 例如，在按设备类型=移动设备进行筛选时，询问投放率是未定义的查询，因为Marketo不会收到基础投放和已发送事件的任何参与量度。 我们正在探索从参与量度中应用设备类型和设备操作系统的方法，以匹配包含参与和交付量度的比率。

## 当某些电子邮件客户端阻止图像时，电子邮件分析会执行什么操作？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一个常见的行业问题是，越来越多的电子邮件客户端默认关闭了图像。 加载图像是记录打开次数的基础。 用户完全有可能收到一封电子邮件，其中图像被阻止，但文本和链接完全可读。 如果用户遇到这种情况，点击了该电子邮件中的链接，您最终可能会遇到点击事件场景，但不会收到针对该电子邮件的相应的“打开”事件。 Marketo电子邮件分析将自动生成任何缺失的事件。 该逻辑与Marketo为电子邮件性能报表以及Revenue Explorer中的电子邮件分析区域执行此操作的方式相同。
