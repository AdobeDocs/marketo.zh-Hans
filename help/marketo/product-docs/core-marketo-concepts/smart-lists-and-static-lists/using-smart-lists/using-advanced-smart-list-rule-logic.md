---
unique-page-id: 1146901
description: 使用高级智能列表规则逻辑 — Marketo文档 — 产品文档
title: 使用高级智能列表规则逻辑
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 使用高级智能列表规则逻辑{#using-advanced-smart-list-rule-logic}

通过将智能列表规则逻辑应用到智能列表中的多个过滤器，您可以找到所需的准确人员。 下面介绍如何操作。

>[!PREREQUISITES]
>
>* [查找过滤器并将其添加到智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [定义智能列表过滤器](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>高级过滤器逻辑仅在智能列表中有三个或更多过滤器时可用。

## 将逻辑添加到智能列表{#add-logic-to-a-smart-list}

默认情况下，您的智能列表将找到与&#x200B;**ALL**&#x200B;过滤器(过滤器1 _和_ 2 _和_ 3)匹配的人员。 您可以更改规则逻辑，以查找符合所定义过滤器的&#x200B;**ANY**&#x200B;的人员(过滤器1 _或_ 2 _或_ 3)，或使用高级过滤器(过滤器1 _和_ 2 _或_ 3)。

在此示例中，假设您要查找加利福尼亚&#x200B;_和_&#x200B;中得分至少为50分的人员&#x200B;_或_，状态为“Sales Qualified”。

1. 从下拉菜单中选择&#x200B;**使用高级过滤器**。

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用&#x200B;**高级**&#x200B;过滤器可减少使用智能列表滤镜成员创建智能列表的需求。 这有助于优化性能。

1. **高级过滤器**&#x200B;文本框将显示“和”作为所有过滤器之间的默认值。

   ![](assets/two-2.png)

1. 在“2”和“3”周围键入一对圆括号。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >输入规则逻辑时，必须在“或”前使用“和”。

1. 将“2”和“3”之间的“和”更改为“或”。

   ![](assets/four-1.png)

## 混合&quot;And&quot;和&quot;或{#use-parentheses-when-mixing-and-and-or}时使用括号

混合“和”和“或”逻辑需要用括号来明确您的意图。

![](assets/advancedfilters-parent.png)

## 如果需要{#use-nested-parentheses-for-four-or-more-filters-if-needed}，请对四个或多个过滤器使用嵌套括号

根据您的意图，在使用四个或更多过滤器时，您可能需要添加嵌套的括号。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>如果输入无效规则，则在该规则下将显示一条红线。 滚动文本以查看相关的错误消息。
