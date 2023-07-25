---
unique-page-id: 1147017
description: 创建任务 — Marketo文档 — 产品文档
title: 创建任务
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 0%

---

# 创建任务 {#create-task}

作为营销人员，您拥有的信息可以帮助销售人员完成交易。 您可以创建任务，以告知他们应该做什么以及何时应该做。

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>Marketo同步用户创建任务时， **到期时间** 是在Salesforce中创建任务的必填字段。 如果没有值，Marketo将默认输入5天。

默认情况下，流程步骤将如下所示：

![](assets/image2014-9-22-14-3a54-3a49.png)

自定义所有字段以您希望的方式创建任务。

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`， `{{company.tokens}}`， `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **主题** 和 **描述**. 参见 [流步骤的令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) 了解更多详细信息。
