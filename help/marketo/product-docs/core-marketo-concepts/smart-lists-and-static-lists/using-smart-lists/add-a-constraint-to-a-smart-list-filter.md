---
unique-page-id: 2949413
description: 向智能列表过滤器添加限制 — Marketo文档 — 产品文档
title: 向智能列表筛选器添加约束
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# 向智能列表筛选器添加约束 {#add-a-constraint-to-a-smart-list-filter}

创建智能列表时，某些过滤器具有称为“约束”的高级选项。 这些是可添加到筛选器和触发器的额外条件，有助于进一步缩小搜索范围。

在此示例中，我们将一些约束添加到&#x200B;**[数据值已更改](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}**&#x200B;筛选器以查找状态从MQL更改为SQL的人员。

>[!PREREQUISITES]
>
>* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [在智能列表中使用“数据值已更改”筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. 转到&#x200B;**[!UICONTROL 营销活动]**。

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. 选择带有要向其添加约束的过滤器的智能列表，然后单击&#x200B;**[!UICONTROL 智能列表]**&#x200B;选项卡。

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. 在&#x200B;**[!UICONTROL 添加约束]**&#x200B;下，选择&#x200B;**[!UICONTROL 上一个值]**。

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. 输入&#x200B;**[!UICONTROL 前一个值]**。 在此示例中，我们使用的是MQL。

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. 在&#x200B;**[!UICONTROL 添加约束]**&#x200B;下，选择&#x200B;**[!UICONTROL 新值]**。

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. 输入新值。 在本例中，我们使用的是SQL。

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. 做得好！ 单击&#x200B;**[!UICONTROL 人员]**&#x200B;选项卡可查看过去30天内具有从“MQL”更改为“SQL”状态的所有人员。
