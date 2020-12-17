---
unique-page-id: 1146950
description: 等待- Marketo Docs —— 产品文档
title: 等待
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# 等待{#wait}

## 概述{#overview}

使用方便的&#x200B;**等待步骤**&#x200B;暂停智能活动流中的人员。

![](assets/wait-overview.png)

注意如何输入自然语言，如“4小时”。 但是，请&#x200B;**不要**&#x200B;缩写单词（即4小时）。 智能活动仍会运行，但等待步骤将被忽略。

>[!CAUTION]
>
>更改等待步骤的持续时间不会影响已输入该步骤的人员。 例如：您有5天的等待步骤，人员进入该步骤，然后您将等待步骤更改为7天——该人员仍只等待原来的5天，然后才能进入下一个流程步骤。

>[!TIP]
>
>如果有人已经在等待步骤中，而不希望他们在等待期结束后继续，请在等待步骤后插入[从流](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)中删除。 使用[添加选择](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md)选项指定要删除的人。

## 用法{#usage}

使用等待流步骤有三种主要方式：

1. [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流程步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
