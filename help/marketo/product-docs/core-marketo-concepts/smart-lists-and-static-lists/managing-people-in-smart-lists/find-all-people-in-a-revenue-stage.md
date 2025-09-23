---
unique-page-id: 557331
description: 查找收入阶段的所有人员 — Marketo文档 — 产品文档
title: 查找处于某收入阶段的所有人员
exl-id: aa5b30bf-96f1-4c1f-8170-86ba808e9705
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 10%

---

# 查找处于某收入阶段的所有人员 {#find-all-people-in-a-revenue-stage}

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

## 查找特定收入阶段的所有成员 {#find-all-members-of-a-specific-revenue-stage}

1. 在智能列表中，单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡，找到&#x200B;**[!UICONTROL Revenue Stage]**&#x200B;筛选器，然后将其拖到画布中。

   ![](assets/draginrevenuefilter.png)

1. 选择&#x200B;**[!UICONTROL Revenue Stage]**。

   ![](assets/two.jpg)

1. 转到&#x200B;**[!UICONTROL People]**&#x200B;选项卡以查看结果。

   ![](assets/peopleresults.jpg)

## 对收入阶段成员运行流程步骤 {#run-a-flow-step-on-the-members-of-a-revenue-stage}

现在您已经知道哪些人处于收入阶段，您可以直接向他们进行营销。 除了选择&#x200B;**[!UICONTROL Revenue Stage]**&#x200B;作为智能列表筛选器外，您还可以将其选为流中的“if”筛选器。

1. 在所需的流程步骤中，单击&#x200B;**[!UICONTROL Add Choice]**&#x200B;并从下拉列表中选择&#x200B;**[!UICONTROL Revenue Stage]**。

   ![](assets/six.png)

   从那里，您可以选择哪些成员受流程步骤的哪个方面影响。
