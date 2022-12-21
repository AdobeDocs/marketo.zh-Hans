---
unique-page-id: 1147001
description: 使用标准智能列表规则逻辑 — Marketo文档 — 产品文档
title: 使用标准智能列表规则逻辑
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用标准智能列表规则逻辑 {#using-standard-smart-list-rule-logic}

在生成营销活动智能列表时，您可能已注意到“使用过滤器”选项。 此设置允许您决定是否需要使用AND或OR运算符来评估过滤器。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>更改智能列表规则逻辑仅适用于过滤器、 **not** 触发器。

即使将上述设置设置为ALL，触发器也始终评估为OR。  以下是一个示例：

![](assets/image2014-9-22-14-3a12-3a57.png)

以下简单的说法是：

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

如果一个人填了表格 **或** 访问页面时，营销活动将根据该人员的评估 **全部** 或 **any** 后续过滤器的数量，具体取决于所使用的设置。

>[!MORELIKETHIS]
>
>[使用高级智能列表规则逻辑](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
