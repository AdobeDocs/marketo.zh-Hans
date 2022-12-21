---
unique-page-id: 1147017
description: 创建任务 — Marketo文档 — 产品文档
title: 创建任务
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 0%

---

# 创建任务 {#create-task}

作为营销人员，您可以获得有助于销售人员完成交易的信息。 您可以创建任务，以告知他们应该执行哪些操作以及何时执行。

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>当Marketo同步用户创建任务时， **到期** 是要在Salesforce中创建的任务的必填字段。 如果没有值，则Marketo默认将输入五天。

默认情况下，流程步骤将如下所示：

![](assets/image2014-9-22-14-3a54-3a49.png)

自定义所有字段，以按所需方式创建任务。

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>您可以使用 `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` 和 `{{system.tokens}}` 在 **主题** 和 **描述**. 请参阅 [用于流量步骤的令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) 以了解更多详细信息。
