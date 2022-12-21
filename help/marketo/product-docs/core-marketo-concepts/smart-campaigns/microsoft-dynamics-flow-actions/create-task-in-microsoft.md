---
unique-page-id: 37356429
description: 在Microsoft中创建任务 — Marketo文档 — 产品文档
title: 在Microsoft中创建任务
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 在Microsoft中创建任务 {#create-task-in-microsoft}

作为营销人员，您可以获得有助于销售人员完成交易的信息。 您可以创建任务，以告知他们应该执行哪些操作以及何时执行。

在Microsoft中创建任务会在与Microsoft中的人员（潜在客户或联系人）相关的活动下创建一个任务。

>[!NOTE]
>
>此流程步骤将 **仅当与触发器一起使用时才可用**，而不是过滤器。

默认情况下，流程步骤将如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>当Marketo同步用户创建任务时， **到期** 是要在Microsoft中创建的任务的必填字段。 如果未输入值，则Marketo默认将输入五天。

自定义所有字段，以按所需方式创建任务。

![](assets/msd2.png)

>[!NOTE]
>
>在“流程操作”中为任务指定的字段“状态”会更新该字段：Microsoft中的“状态原因”。

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **主题** 和 **描述**. 请参阅 [用于流量步骤的令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) 以了解更多详细信息。
