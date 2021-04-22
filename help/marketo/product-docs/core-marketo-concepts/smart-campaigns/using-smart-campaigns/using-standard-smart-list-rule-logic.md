---
unique-page-id: 1147001
description: 使用标准智能列表规则逻辑 — Marketo文档 — 产品文档
title: 使用标准智能列表规则逻辑
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 使用标准智能列表规则逻辑{#using-standard-smart-list-rule-logic}

在构建活动智能列表时，您可能已注意到“使用过滤器”选项。 此设置允许您决定是否需要使用AND或OR运算符来评估过滤器。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>更改智能列表规则逻辑仅适用于过滤器,**不适用于**&#x200B;触发器。

即使将上述设置设置为ALL，触发器也始终被评估为OR。  以下是一个示例：

![](assets/image2014-9-22-14-3a12-3a57.png)

以上智能列表简言之：

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

因此，如果某个人填写了表单&#x200B;**或**&#x200B;访问页面，则活动将根据后续过滤器的&#x200B;**all**&#x200B;或&#x200B;**any**&#x200B;来评估该人，具体取决于所使用的设置。

>[!MORELIKETHIS]
>
>[使用高级智能列表规则逻辑](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
