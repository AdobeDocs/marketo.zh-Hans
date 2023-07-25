---
unique-page-id: 1147001
description: 使用标准智能列表规则逻辑 — Marketo文档 — 产品文档
title: 使用标准智能列表规则逻辑
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用标准智能列表规则逻辑 {#using-standard-smart-list-rule-logic}

在构建营销活动智能列表时，您可能会注意到“使用过滤器”选项。 通过此设置，可决定是需要使用AND还是OR运算符来评估过滤器。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>更改智能列表规则逻辑仅适用于筛选器， **非** 触发器。

触发器始终被评估为OR，即使以上设置设置为ALL也是如此。  示例如下：

![](assets/image2014-9-22-14-3a12-3a57.png)

以上智能列表用词表示：

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

所以，如果一个人填写了表格 **或** 访问页面，活动将根据以下条件评估该人员 **所有** 或 **任意** 根据使用的设置，选择后续过滤器。

>[!MORELIKETHIS]
>
>[使用高级智能列表规则逻辑](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
