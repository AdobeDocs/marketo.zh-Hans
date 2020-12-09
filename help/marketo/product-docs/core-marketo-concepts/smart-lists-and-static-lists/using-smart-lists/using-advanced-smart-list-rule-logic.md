---
unique-page-id: 1146901
description: 使用高级智能列表规则逻辑- Marketo Docs —— 产品文档
title: 使用高级智能列表规则逻辑
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# 使用高级智能列表规则逻辑 {#using-advanced-smart-list-rule-logic}

通过将智能列表规则逻辑应用于智能列表中的多个过滤器，您可以找到所需的准确人员。 这是方法。

>[!PREREQUISITES]
>
>* [查找过滤器并将其添加到智能列表](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [定义智能列表过滤器](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>



>[!NOTE]
>
>高级过滤器逻辑仅在智能列表中有三个或更多过滤器时可用。

## 将逻辑添加到智能列表 {#add-logic-to-a-smart-list}

默认情况下，您的智能列表将找到与所有过滤器 **匹配** (过滤器1 *和2* 和3 *)* 的人员。 您可以更改规则逻辑，以查找符 **合所定** 义过滤器的任意( *过滤器1或* 2或 *3)、或使用高级过滤器(过滤器1*** 和2或*3)的人员。

在此示例中，假设您想要在加利福尼亚 *找到* 得分至少为50分或 *状态为* “销售合格”的人。

1. 从 **下拉****框** 中选 **择“使用高级** 过滤器”。

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用 **高级过滤器** ，无需使用智能列表过滤器的成员来创建智能列表。 这有助于优化性能。

1. 高 **级** 过滤器 **文本框将显示** “和”作为所有过滤器之间的默认值。

   ![](assets/two-2.png)

1. 在“2”和“3”周围键入一对括号。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >输入规则逻辑时，必须在“或”前使用“和”。

1. 将“2”和“3”之间的“和”更改为“或”。

   ![](assets/four-1.png)

## 混合“和”和“或”时使用括号 {#use-parentheses-when-mixing-and-and-or}

混合“和”和“或”逻辑需要括号来明确您的意图。

![](assets/advancedfilters-parent.png)

## 如果需要，请对四个或更多过滤器使用嵌套括号 {#use-nested-parentheses-for-four-or-more-filters-if-needed}

根据您的意图，您可能需要在使用四个或更多过滤器时添加嵌套括号。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>如果输入无效规则，您将看到规则下方显示一条红线。 滚动到文本上可看到相关错误消息。

