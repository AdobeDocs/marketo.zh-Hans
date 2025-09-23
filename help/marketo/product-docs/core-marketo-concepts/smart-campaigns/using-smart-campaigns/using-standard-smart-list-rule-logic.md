---
unique-page-id: 1147001
description: 使用标准智能列表规则逻辑 — Marketo文档 — 产品文档
title: 使用标准智能列表规则逻辑
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 9%

---

# 使用标准智能列表规则逻辑 {#using-standard-smart-list-rule-logic}

在构建Campaign智能列表时，您可能已经注意到“使用过滤器”选项。 通过此设置，可决定是需要使用AND运算符还是使用OR运算符来评估过滤器。

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>更改智能列表规则逻辑仅适用于筛选器，_不是_&#x200B;触发器。

触发器始终被评估为OR，即使上述设置被设置为ALL也是如此。 示例如下：

![](assets/using-standard-smart-list-rule-logic-2.png)

以上智能列表用词表示：

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

因此，如果某人填写表单&#x200B;_或_&#x200B;访问了该页面，则营销活动将根据&#x200B;_all_&#x200B;或&#x200B;_any_&#x200B;的后续筛选条件评估该人员，具体取决于使用的设置。

>[!MORELIKETHIS]
>
>[使用高级智能列表规则逻辑](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
