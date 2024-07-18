---
unique-page-id: 557316
description: 定义智能列表过滤器 — Marketo文档 — 产品文档
title: 定义智能列表筛选器
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# 定义智能列表筛选器 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [查找筛选器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

现在您已[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}并在其中添加了[筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}，接下来让我们定义筛选器。 具体方法如下。

继续我们的示例，让我们定义这些过滤器以查找得分超过50分的加利福尼亚州所有人员。

1. 转到&#x200B;**[!UICONTROL 营销活动]**。

   ![](assets/define-smart-list-filters-1.png)

1. 选择所需的智能列表，然后单击&#x200B;**[!UICONTROL 智能列表]**&#x200B;选项卡。

   ![](assets/define-smart-list-filters-2.png)

1. 为&#x200B;**[!UICONTROL 状态]**&#x200B;筛选器查找并选择“CA”。

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >您可能同时存储了“加利福尼亚”和“CA”。 为了筛选这两个值并包括加利福尼亚的&#x200B;_所有_&#x200B;人员，了解如何[将多个值添加到智能列表筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}。

1. 选择&#x200B;**[!UICONTROL 大于]**&#x200B;运算符并输入“50”。

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>如果您认为数据库中可能有一些记录包含不完整的电子邮件地址(例如，只有“@adobe.com”)，请在使用“包含”运算符时使用两个电子邮件地址过滤器。 一个带有“contains @adobe.com”的过滤器，和一个带有“contains adobe.com”的单独过滤器（省略@符号）。

现在，您已了解如何创建智能列表并添加/定义筛选器。
