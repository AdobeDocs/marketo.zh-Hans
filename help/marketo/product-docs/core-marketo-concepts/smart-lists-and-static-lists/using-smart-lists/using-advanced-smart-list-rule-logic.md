---
unique-page-id: 1146901
description: 使用高级智能列表规则逻辑 — Marketo文档 — 产品文档
title: 使用高级智能列表规则逻辑
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 使用高级智能列表规则逻辑 {#using-advanced-smart-list-rule-logic}

通过将智能列表规则逻辑应用于智能列表中的多个筛选器，您可以找到所需的确切人员。 具体方法如下。

>[!PREREQUISITES]
>
>* [查找筛选器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [定义智能列表筛选器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>[!NOTE]
>
>仅当智能列表中包含三个或更多过滤器时，高级过滤器逻辑才可用。

## 将逻辑添加到智能列表 {#add-logic-to-a-smart-list}

默认情况下，您的智能列表将查找匹配的人员 **所有** 过滤器(过滤器1 _和_ 2 _和_ 3)。 您可以更改规则逻辑以查找匹配的人员 **任意** 已定义过滤器(过滤器1 _或_ 2 _或_ 3)，或使用高级过滤器(过滤器1 _和_ 2 _或_ 3)。

在此示例中，假设您希望查找加利福尼亚的人员 _和_ 得分至少为50分 _或_ 状态为“销售合格”。

1. 选择 **使用高级过滤器** 从下拉菜单中查找。

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用 **高级** 过滤器可减少使用“智能列表的成员”过滤器创建智能列表的需求。 这有助于优化性能。

1. 此 **高级过滤器** 文本框将显示“和”作为所有筛选器之间的默认值。

   ![](assets/two-2.png)

1. 在“2和3”周围键入一对圆括号。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >输入规则逻辑时，必须在“or”之前使用“and”。

1. 将“2和3”之间的“和”更改为“或”。

   ![](assets/four-1.png)

## 混合“And”和“Or”时使用圆括号 {#use-parentheses-when-mixing-and-and-or}

将“and”和“or”逻辑混合在一起时，需要用括号明确表达您的意图。

![](assets/advancedfilters-parent.png)

## 如果需要，可为四个或更多过滤器使用嵌套括号 {#use-nested-parentheses-for-four-or-more-filters-if-needed}

根据您的意图，在使用四个或更多过滤器时，您可能需要添加嵌套括号。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>如果输入无效的规则，您将看到该规则下显示一条红线。 滚动文本以查看相关的错误消息。
