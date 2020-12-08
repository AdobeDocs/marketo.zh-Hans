---
unique-page-id: 37356429
description: 在Microsoft - Marketo Docs —— 产品文档中创建任务
title: 在Microsoft中创建任务
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# 在Microsoft中创建任务 {#create-task-in-microsoft}

作为营销人员，您可以获得有助于销售完成交易的信息。 您可以创建任务，让他们知道他们应该做什么以及何时应该做。

在Microsoft中创建任务在与Microsoft中的“人员”（潜在客户或联系人）相关的活动下创建任务。

>[!NOTE]
>
>仅当在智能 **活动中与触发器一起使用**，而非与过滤器一起使用时，此流步骤才有效。

默认情况下，流步骤将如下所示：   ![](assets/msd1.png)

>[!NOTE]
>
>当Marketo Sync用户正在创建任务时，**Due In **是要在Microsoft中创建任务的必填字段。 如果未输入值，Marketo将默认输入五天。

自定义所有字段，以您希望的方式创建任务。   ![](assets/msd2.png)

>[!NOTE]
>
>为“流动操作”中的任务指定的字段“状态”将更新该字段：Microsoft中的“状态原因”。

>[!TIP]
>
>您可以在主 `{{lead.tokens}}`题和 `{{company.tokens}}`说明 `{{campaign.tokens}}` 中使 `{{system.tokens}}` 用、以 **及** 在中 ****&#x200B;使用。 有关更 [多详细信息，请参](http://docs.marketo.com/x/c4AR) 阅流步骤令牌。

