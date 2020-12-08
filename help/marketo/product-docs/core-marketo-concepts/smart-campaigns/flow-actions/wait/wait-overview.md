---
unique-page-id: 1146950
description: 等待- Marketo Docs —— 产品文档
title: 等待
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 等待 {#wait}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](/help/marketo/getting-started/updates-to-marketo-terminology.md)。

## 概述 {#overview}

通过方便的等待步骤，在智能活动流中暂 **停人员**。

![](assets/wait-overview.png)

注意如何输入自然语言，如“4小时”。 但 **是**，请勿将这些单词缩写（即4小时）。 智能活动仍会运行，但等待步骤将被忽略。

>[!CAUTION]
>
>更改等待步骤的持续时间不会影响已输入该步骤的人员。 例如：您有5天的等待步骤，人员进入该步骤，然后您将等待步骤更改为7天——该人员仍只等待原来的5天，然后才能进入下一个流程步骤。

>[!TIP]
>
>如果有人已经在等待步骤中，而不希望他们在等待期结束后继续，请在等待 [步骤后](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) ，直接插入“从流中删除”。 使用“添加选择”选项指定 [要删除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) 的人。

## 使用情况 {#usage}

使用等待流步骤有三种主要方式：

1. [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流程步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
