---
unique-page-id: 37356429
description: 在Microsoft - Marketo Docs — 产品文档中创建任务
title: 在Microsoft中创建任务
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 在Microsoft {#create-task-in-microsoft}中创建任务

作为营销人员，您拥有可帮助销售人员达成交易的信息。 您可以创建任务，让他们知道他们应该做什么以及何时应该做。

在Microsoft中创建任务在与Microsoft中的“人员（潜在客户或联系人）”相关的活动下创建任务。

>[!NOTE]
>
>仅当在智能活动中与触发器&#x200B;**一起使用时，此流步骤才**&#x200B;起作用，而不是过滤器。

默认情况下，流步骤将如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>当Marketo同步用户创建任务时，**Due In**&#x200B;是要在Microsoft中创建任务的必填字段。 如果未输入值，Marketo将默认输入五天。

自定义所有字段，以您希望的方式创建任务。

![](assets/msd2.png)

>[!NOTE]
>
>在“流操作”中为任务指定的字段“状态”更新了该字段：Microsoft中的“状态原因”。

>[!TIP]
>
>可以在&#x200B;**Subject**&#x200B;和&#x200B;**Description**&#x200B;中使用`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`和`{{system.tokens}}`。 有关详细信息，请参阅[流步骤令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)。
