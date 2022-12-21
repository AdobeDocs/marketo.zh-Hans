---
unique-page-id: 10100257
description: 电子邮件分析常见问题解答 — Marketo文档 — 产品文档
title: 电子邮件分析常见问题解答
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# 电子邮件分析常见问题解答 {#email-insights-faq}

## 电子邮件分析与其他Marketo电子邮件报表中的比率量度之间是否有任何差异？ {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

是. 电子邮件分析可将参与度量度与它们对应的投放量度关联，以用于计算参与度量度比率（打开率、点击至打开率、取消订阅率）时发送的相同电子邮件。 例如，在电子邮件分析中，当查看过去一周包含点击至打开率每日划分的时间系列图表时，我们现在会根据相应的投放量度显示打开/点击/取消订阅事件的真正相关比率。 这与收入浏览器中的行为形成了鲜明对比，后者只是对所有内容进行汇总。 电子邮件分析可以更准确地查看参与率。

## 为什么电子邮件分析仅支持10个自定义Dimension? {#why-does-email-insights-only-support-custom-dimensions}

对于许多用例，使用10个附加的自定义维度扩展默认系统维度将远远不够，并且包括基于分段或项目标记的自定义维度。 将来，我们计划允许客户增加允许的自定义Dimension数量。

## 为什么在分配自定义Dimension版块后无法重新使用它们？ {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

分配给定的自定义Dimension插槽后，重新映射该插槽会导致以前的数据与新含义混合时产生错误。 因此，不能重复使用自定义Dimension插槽。 此行为与其他量度分析工具(如Google Analytics)的行为一致。

## 电子邮件分析是否支持Marketo Sales Insight电子邮件？ {#does-email-insights-support-marketo-sales-insight-emails}

是. 通过Marketo销售分析发送的所有电子邮件都包含在电子邮件分析中。

## 电子邮件分析是否支持操作电子邮件？ {#does-email-insights-support-operational-emails}

是. 默认情况下，操作电子邮件会隐藏起来，无法查看和查询。 但是，您可以在“个人设置”面板下更改此设置。

## 电子邮件分析是否会捕获定期计划或重新运行的智能促销活动电子邮件流程步骤？ {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

是和否。 在电子邮件分析的初始版本中，可以捕获所有电子邮件事件，并可对任何定期计划或重新运行的智能营销活动访问这些事件。 但您无法区分该智能营销活动的不同运行方式。 我们将在下一版本中添加支持，以捕获打开、点击和取消订阅事件的智能营销活动运行信息，以便区分这些事件。

## 为什么我按设备类型或设备操作系统进行过滤时，许多量度显示为零？ {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除“点击至打开率”、“打开数”、“点击数”和“取消订阅数”之外，所有其他受支持的量度均为投放事件或从投放事件派生的比率。 由于设备类型和设备操作系统仅适用于参与度量度，因此我们根本没有要显示的信息。 例如，按设备类型= mobile过滤后，这是一个未定义的查询，用于要求提供交付率，因为Marketo不会收到基础交付和已发送事件的任何参与量度。 我们正在探索如何从参与度量度中应用设备类型和设备操作系统，以获得包含参与度和交付度量度的比率。

## 当某些电子邮件客户端阻止图像时，电子邮件分析会有什么作用？ {#what-does-email-insights-do-when-certain-email-clients-block-images}

一个常见的行业问题是，越来越多的电子邮件客户默认关闭图像。 加载图像是记录打开次数的基础。 用户完全可能会收到一封包含被阻止图像的电子邮件，但其文本和链接完全可读。 如果用户经历此情况并点击了该电子邮件中的链接，则最终会出现“点击”事件的情景，但没有针对该电子邮件的相应“打开”事件。 Marketo电子邮件分析将自动生成任何缺失的事件。 其逻辑与Marketo如何对“电子邮件性能”报表执行此操作以及收入资源管理器中的“电子邮件分析”区域执行此操作相同。
