---
unique-page-id: 1146950
description: 等待 — Marketo文档 — 产品文档
title: 等待
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# 等待 {#wait}

## 概述 {#overview}

使用方便项暂停智能营销活动流中的人员 **等待步骤**.

![](assets/wait-overview.png)

请注意如何键入自然语言，如“4小时”。 Do **非**&#x200B;但是，缩写这些字（即4小时）。 明智的竞选活动仍将运行，但等待步骤将被忽略。

>[!CAUTION]
>
>更改等待步骤的持续时间不会影响已进入该步骤的人员。 例如：您有一个等待步骤5天，人员进入该步骤，然后您将等待步骤更改为7天 — 该人员仍然只会等待原来的5天，然后再进入下一个流量步骤。

>[!TIP]
>
>如果您已有人处于等待步骤，并且不希望他们在等待期结束后前进，请插入 [从流中删除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) 就在等待步骤之后。 使用指定要删除的人员 [添加选项](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) 选项。

## 使用情况 {#usage}

可以使用等待流步骤的三种主要方式：

1. [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
