---
unique-page-id: 557316
description: 了解如何定义智能列表筛选器。 设置过滤器约束和值以确定列表中显示的对象。
title: 定义智能列表过滤器
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/gCJT14FtnJaPAMhDUWI7XpoST1lc9yvzZbVKq-oTx-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 5%
---
# 定义智能列表过滤器 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [查找筛选器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

现在您已[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}并在其中添加了[筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}，请按照以下方式定义筛选器。

继续此示例，定义这些过滤器以查找得分超过50分的加利福尼亚州所有人员。

1. 前往 **[!UICONTROL Marketing Activities]**。

   ![](assets/define-smart-list-filters-1.png)

1. 选择所需的智能列表，然后单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/define-smart-list-filters-2.png)

1. 为&#x200B;**[!UICONTROL State]**&#x200B;筛选器查找并选择“CA”。

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >您可能同时存储了“加利福尼亚”和“CA”。 为了筛选这两个值并包括加利福尼亚的&#x200B;_所有_&#x200B;人员，了解如何[将多个值添加到智能列表筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}。

1. 选择&#x200B;**[!UICONTROL greater than]**&#x200B;运算符并输入“50”。

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>如果您认为数据库中可能有一些记录包含不完整的电子邮件地址（例如，只有“@adobe.com”），请在使用“包含”运算符时使用两个电子邮件地址过滤器。 一个带有“contains @adobe.com”的过滤器，和一个带有“contains adobe.com”的单独过滤器（省略@符号）。

现在，您已了解如何创建智能列表并添加/定义筛选器。
