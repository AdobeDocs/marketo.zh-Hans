---
unique-page-id: 1147017
description: 了解如何在流程步骤中创建Salesforce任务。 在人员进入流程时为潜在客户责任人创建任务。
title: 创建任务
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/RJ5nZrVvURtgXEWWZwL2xXzlYOhWjKGSbX-MFTWCwzg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 126
ht-degree: 3%

---

# 创建任务 {#create-task}

作为营销人员，您掌握的信息可帮助销售人员完成交易。 您可以创建任务，以告知他们应该做什么以及何时应该做什么。

![](assets/create-task-1.png)

>[!NOTE]
>
>当Marketo同步用户创建任务时，**[!UICONTROL Due In]**&#x200B;是要在Salesforce中创建任务的必填字段。 如果没有值，Marketo将默认输入5天。

默认情况下，流程步骤将如下所示：

![](assets/create-task-2.png)

自定义所有字段以您希望的方式创建任务。

![](assets/create-task-3.png)

>[!TIP]
>
>您可以在&#x200B;**[!UICONTROL Subject]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;中使用`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`和`{{system.tokens}}`。 有关更多详细信息，请参阅流程步骤[令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}。
