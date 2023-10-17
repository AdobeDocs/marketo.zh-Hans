---
unique-page-id: 37356429
description: 在Microsoft中创建任务 — Marketo文档 — 产品文档
title: 在Microsoft中创建任务
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 在Microsoft中创建任务 {#create-task-in-microsoft}

作为营销人员，您掌握的信息可帮助销售人员完成交易。 您可以创建任务，以告知他们应该做什么以及何时应该做什么。

在Microsoft中创建任务会在中与人员（潜在客户或联系人）相关的活动下创建任务。 [!DNL Microsoft].

>[!NOTE]
>
>此流程步骤将 _仅当与触发器一起使用时才有效_，而不是过滤器。

默认情况下，流程步骤将如下所示：

![](assets/msd1.png)

>[!NOTE]
>
>当Marketo同步用户创建任务时， **[!UICONTROL 到期时间]** 是要在中创建的任务的必填字段 [!DNL Microsoft]. 如果未输入值，Marketo将默认输入5天。

自定义所有字段以您希望的方式创建任务。

![](assets/msd2.png)

>[!NOTE]
>
>在“流程操作”中为任务指定的“状态”字段更新了中的“状态原因” [!DNL Microsoft].

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`， `{{company.tokens}}`， `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **[!UICONTROL 主题]** 和 **[!UICONTROL 描述]**. 请参阅 [流程步骤的令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} 以了解更多详细信息。
