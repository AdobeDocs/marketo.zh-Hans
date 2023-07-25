---
unique-page-id: 37356429
description: 在Microsoft中创建任务 — Marketo文档 — 产品文档
title: 在Microsoft中创建任务
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 在Microsoft中创建任务 {#create-task-in-microsoft}

作为营销人员，您拥有的信息可以帮助销售人员完成交易。 您可以创建任务，以告知他们应该做什么以及何时应该做。

在Microsoft中创建任务可在Microsoft中与人员（潜在客户或联系人）相关的活动下创建任务。

>[!NOTE]
>
>此流程步骤将 **仅当与触发器一起使用时才有效**，而不是过滤器。

默认情况下，流程步骤将如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>Marketo同步用户创建任务时， **到期时间** 是要在Microsoft中创建的任务的必填字段。 如果未输入值，Marketo将默认输入5天。

自定义所有字段以您希望的方式创建任务。

![](assets/msd2.png)

>[!NOTE]
>
>在“流程操作”中为任务指定的“状态”字段会更新Microsoft中的“状态原因”字段。

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`， `{{company.tokens}}`， `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **主题** 和 **描述**. 参见 [流步骤的令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) 了解更多详细信息。
