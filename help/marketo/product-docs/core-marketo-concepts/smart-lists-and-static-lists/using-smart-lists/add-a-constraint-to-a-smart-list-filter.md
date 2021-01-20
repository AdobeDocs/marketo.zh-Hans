---
unique-page-id: 2949413
description: 向智能列表过滤器- Marketo Docs —— 产品文档添加约束
title: 向智能列表滤镜添加约束
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# 向智能列表过滤器{#add-a-constraint-to-a-smart-list-filter}添加约束

创建智能列表时，某些过滤器具有称为“约束”的高级选项。 这些是可添加到过滤器和触发器的额外条件，有助于进一步缩小搜索范围。

在此示例中，让我们向&#x200B;**[数据值已更改](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**&#x200B;过滤器添加一些约束，以查找状态从MQL更改为SQL的人员。

>[!PREREQUISITES]
>
>* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [在智能列表中使用“数据值已更改”筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. 转到&#x200B;**营销活动**。

   ![](assets/ma-1.png)

1. 选择带有要向其添加约束的筛选器的智能列表，然后单击&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/two-3.png)

1. 在&#x200B;**添加约束**&#x200B;下，选择&#x200B;**上一值**。

   ![](assets/three-3.png)

1. 输入&#x200B;**上一个值**。 在此示例中，我们使用MQL。

   ![](assets/four-2.png)

1. 在&#x200B;**添加约束**&#x200B;下，选择&#x200B;**新值**。

   ![](assets/five.png)

1. 输入&#x200B;**新值**。 在本示例中，我们使用SQL。

   ![](assets/six.png)

1. 干得好！ 单击&#x200B;**People**&#x200B;选项卡，查看过去30天中具有&#x200B;**Status**&#x200B;从&#x200B;**MQL**&#x200B;更改为&#x200B;**SQL**&#x200B;的所有人员。
