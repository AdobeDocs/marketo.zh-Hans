---
unique-page-id: 2949413
description: 向智能列表过滤器添加约束 — Marketo文档 — 产品文档
title: 向智能列表筛选器添加约束
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# 向智能列表筛选器添加约束 {#add-a-constraint-to-a-smart-list-filter}

创建智能列表时，某些过滤器具有称为“约束”的高级选项。 这些是可添加到过滤器和触发器的额外条件，可帮助进一步缩小搜索范围。

在本例中，让我们向 **[数据值已更改](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** 过滤器以查找状态从MQL更改为SQL的人员。

>[!PREREQUISITES]
>
>* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [在智能列表中使用“数据值已更改”过滤器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>


1. 转到 **营销活动**.

   ![](assets/ma-1.png)

1. 选择要添加约束的筛选器的智能列表，然后单击 **智能列表** 选项卡。

   ![](assets/two-3.png)

1. 在 **添加约束**，选择 **上一值**.

   ![](assets/three-3.png)

1. 输入 **上一值**. 在本例中，我们使用的是MQL。

   ![](assets/four-2.png)

1. 在 **添加约束**，选择 **新值**.

   ![](assets/five.png)

1. 输入 **新值**. 在本例中，我们使用的是SQL。

   ![](assets/six.png)

1. 干得好！ 单击 **人员** 选项卡，查看 **状态** 更改 **MQL** to **SQL** 过去30天里。
