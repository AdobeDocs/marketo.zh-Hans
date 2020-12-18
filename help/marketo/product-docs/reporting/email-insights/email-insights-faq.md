---
unique-page-id: 10100257
description: 电子邮件洞察常见问题解答——营销文档——产品文档
title: 电子邮件洞察常见问题解答
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# 电子邮件洞察常见问题解答{#email-insights-faq}

## 电子邮件洞察和其他营销人员电子邮件报告中的比率指标之间是否存在差异？{#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

是的。 电子邮件洞察将参与度指标与其在计算参与度指标比率（开放率、点击至开放率、取消订阅率）时发送的相同电子邮件的相应投放指标关联起来。 例如，在“电子邮件分析”中，当查看过去一周包含点击至开放率每日细分的时间序列图表时，我们现在会根据相应的事件量度显示打开／点击／取消订阅投放的真实相关比率。 这与收入浏览器中的行为形成了鲜明对比，后者只是将所有内容总和。 电子邮件洞察可更准确地视图参与率。

## 为什么电子邮件洞察只支持10个自定义Dimension?{#why-does-email-insights-only-support-custom-dimensions}

对于许多用例，使用10个附加的自定义尺寸扩展默认系统尺寸将绰绰有余，并包含基于细分或项目标记的自定义尺寸。 未来，我们计划允许客户增加允许的自定义Dimension数。

## 为什么分配自定义Dimension插槽后无法重新使用它们？{#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

一旦分配了给定的自定义Dimension槽，重新映射它将导致以前数据与新含义混合时产生错误。 因此，不能重新使用自定义Dimension插槽。 此行为与其他度量分析工具(如Google Analytics)的行为一致。

## Email Insights是否支持Marketo Sales Insight电子邮件？{#does-email-insights-support-marketo-sales-insight-emails}

是的。 通过Marketo Sales Insights发送的所有电子邮件都包含在Email Insights中。

## 电子邮件洞察是否支持运营电子邮件？{#does-email-insights-support-operational-emails}

是的。 默认情况下，操作电子邮件会隐藏起来，不会视图和查询。 但是，您可以在“个人设置”面板下更改此设置。

## 电子邮件洞察是捕获重复的计划或重新运行智能活动电子邮件流程步骤？{#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

是和否。 在电子邮件洞察的初始版本中，所有电子邮件事件均可被捕获，并可针对任何重复的计划或重新运行的智能活动进行访问。 但您无法区分该智能活动的不同版本。 我们将在下一版本中添加支持，以捕获“打开”、“单击”和“取消订阅”活动的智能事件运行信息，以便与众不同。

## 为什么按设备类型或设备操作系统进行筛选时，许多指标显示为零？{#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

除“点击至开放率”、“打开”、“点击”和“取消订阅”之外，所有其他支持的指标都是投放事件或从投放事件派生的比率。 由于设备类型和设备操作系统仅适用于参与度指标，因此我们根本没有要显示的信息。 例如，按设备类型= mobile筛选时，它是一个未定义的查询请求投放率，因为Marketo不会收到基础投放和已发送事件的任何参与量度。 我们正在探索如何从“参与”指标中对包括“参与”和“投放”指标的比率应用设备类型和设备操作系统。

## 当某些电子邮件客户阻止图像时，Email Insights有何作用？{#what-does-email-insights-do-when-certain-email-clients-block-images}

一个常见的行业问题是，越来越多的电子邮件客户默认关闭图像。 加载图像是记录“打开”的基础。 用户完全可能会收到一封电子邮件，其中图像被阻止，但文本和链接完全可读。 如果用户遇到此问题并单击了该电子邮件中的链接，您会遇到单击事件的情况，但该电子邮件没有相应的打开事件。 Marketo电子邮件洞察将自动生成任何缺失的事件。 其逻辑与Marketo如何对“电子邮件性能”报告以及收入浏览器中的“电子邮件分析”区域执行此操作相同。
