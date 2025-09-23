---
unique-page-id: 37356429
description: 在Microsoft中创建任务 — Marketo文档 — 产品文档
title: 在 Microsoft 中创建任务
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 4%

---

# 在 Microsoft 中创建任务 {#create-task-in-microsoft}

作为营销人员，您掌握的信息可帮助销售人员完成交易。 您可以创建任务，以告知他们应该做什么以及何时应该做什么。

在Microsoft中创建任务会在[!DNL Microsoft]中与人员（潜在客户或联系人）相关的活动下创建任务。

>[!NOTE]
>
>此流程步骤&#x200B;_仅在您的智能营销活动中与触发器_&#x200B;一起使用（而非过滤器）时才有效。

默认情况下，流程步骤将如下所示：

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>当Marketo同步用户创建任务时，**[!UICONTROL Due In]**&#x200B;是将在[!DNL Microsoft]中创建的任务的必填字段。 如果未输入值，Marketo将默认输入5天。

自定义所有字段以您希望的方式创建任务。

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>在“流程操作”中为任务指定的“状态”字段更新了[!DNL Microsoft]中的“状态原因”字段。

>[!TIP]
>
>您可以在`{{lead.tokens}}`和`{{company.tokens}}`中使用`{{campaign.tokens}}`、`{{system.tokens}}`、**[!UICONTROL Subject]**&#x200B;和&#x200B;**[!UICONTROL Description]**。 有关更多详细信息，请参阅流程步骤[令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}。
