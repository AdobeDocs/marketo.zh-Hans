---
unique-page-id: 1146950
description: 等待 — Marketo文档 — 产品文档
title: 等待
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 等待概述 {#wait-overview}

使用方便的&#x200B;**等待步骤**&#x200B;在Smart Campaign流中暂停人员。

![](assets/wait-overview-1.png)

请注意如何键入自然语言，如“4小时”。 请&#x200B;**不要**，但是，请缩写单词（即4小时）。 智能营销活动仍会运行，但等待步骤将被忽略。

>[!CAUTION]
>
>更改等待步骤的持续时间不会影响已进入该步骤的人员。 例如：您有一个等待步骤5天，人员进入该步骤，然后您将等待步骤更改为7天 — 该人员仍然只等待原来的5天，然后再进入下一个流量步骤。

>[!TIP]
>
>如果有人已经在等待步骤中，并且不希望他们在等待时段结束后前进，请在等待步骤之后立即插入[从流](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)中删除。 使用[添加选项](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md)选项指定要删除的人员。

使用等待流步骤的主要方法有三种：

1. [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [在等待流步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
