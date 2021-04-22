---
unique-page-id: 1146950
description: 等待 — Marketo Docs — 产品文档
title: 等
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 等待{#wait}

## 概述{#overview}

使用方便的&#x200B;**等待步骤**&#x200B;暂停智能活动流中的人员。

![](assets/wait-overview.png)

注意，您如何以“4小时”等自然语言输入。 但是，请&#x200B;**不**&#x200B;缩写单词（即4小时）。 智能活动仍将运行，但等待步骤将被忽略。

>[!CAUTION]
>
>更改等待步骤的持续时间不会影响已输入该步骤的人员。 例如：等待步骤为5天，人员进入该步骤，然后您将等待步骤更改为7天 — 该人仍然只等待原始的5天，然后才进入下一个流步骤。

>[!TIP]
>
>如果您有人已经在等待步骤中，并且不希望他们在等待期结束后继续，请在等待步骤后插入[从流](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)中删除。 使用[添加选择](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md)选项指定要删除的对象。

## 用法{#usage}

使用等待流步骤有三种主要方式：

1. [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流程步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
