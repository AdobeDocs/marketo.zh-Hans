---
unique-page-id: 557316
description: 定义智能列表过滤器 — Marketo文档 — 产品文档
title: 定义智能列表筛选器
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 定义智能列表筛选器 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [创建智能列表](create-a-smart-list.md)
>* [查找筛选器并将其添加到智能列表](find-and-add-filters-to-a-smart-list.md)

既然你已经 [已创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 和 [已添加筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) 为此，让我们定义过滤器。 下面是具体操作方法。

继续我们的示例，让我们定义这些过滤器以查找得分超过50分的加利福尼亚州的所有人。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-1.png)

1. 选择智能列表，然后单击 **智能列表** 选项卡。

   ![](assets/smarlist-choosefilters.png)

1. 查找并选择 **CA** 对于 **状态** 筛选条件。

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >您可能存储了这两个 **加利福尼亚** 和 **CA**. 要筛选两个值和包含，请执行以下操作 _所有_ 加州人，学习如何  [向智能列表筛选器添加多个值](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. 选取 **大于** 运算符并输入 **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>如果您认为数据库中的某些记录包含不完整的电子邮件地址(例如，只有“@adobe.com”)，请使用 **二** 使用“包含”运算符时的电子邮件地址过滤器。 一个过滤器使用“包含@adobe.com”，另一个过滤器使用“包含adobe.com”（省略@符号）。

您现在知道如何创建智能列表和添加/定义筛选器。
