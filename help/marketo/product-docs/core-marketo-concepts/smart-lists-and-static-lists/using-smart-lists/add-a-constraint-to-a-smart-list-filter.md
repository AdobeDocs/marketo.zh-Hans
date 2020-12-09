---
unique-page-id: 2949413
description: 向智能列表过滤器- Marketo Docs —— 产品文档添加约束
title: 向智能列表滤镜添加约束
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# 向智能列表滤镜添加约束 {#add-a-constraint-to-a-smart-list-filter}

创建智能列表时，某些过滤器具有名为*constraints的高级选项。 *您可以向过滤器和触发器添加这些附加条件，以帮助进一步缩小搜索范围。

在此示例中，让我们向**数据值已更 [改*](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)*过滤器添加一些约束，以查找状态从MQL更改为SQL的人员。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!PREREQUISITES]
>
>* [创建智能列表](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [在智能列表中使用“数据值已更改”筛选器](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. 转到营 **销活动**。

   ![](assets/ma-1.png)

1. 选择带有要向其添加约束的筛选器的智能列表，然后单击“智 **能列表** ”选项卡。

   ![](assets/two-3.png)

1. 在“添 **加约束**”(Add Constraint **)下，选**&#x200B;择“上一值”(Previous Value)。

   ![](assets/three-3.png)

1. 输入上 **一个值**。 在此示例中，我们使用MQL。

   ![](assets/four-2.png)

1. 在“添 **加约束**”下，选 **择“新值”**。

   ![](assets/five.png)

1. 输入 **新值**。 在本示例中，我们使用SQL。

   ![](assets/six.png)

1. 干得好！ 单击“ **人员** ”选项卡，查看状态从MQL更改为过去30 **天中** SQL状态的 ******** 所有人员。

