---
description: 在Velocity脚本 — Marketo Docs — 产品文档中更改自定义对象检索限制
title: 在速度脚本中更改自定义对象检索限制
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 在速度脚本{#change-custom-object-retrieval-limits-in-velocity-scripting}中更改自定义对象检索限制

如果您使用Velocity脚本在电子邮件中显示自定义对象数据，则此功能可能适合您。 默认情况下，允许您从Velocity Script访问10个父自定义对象。 如果您需要访问更多内容，请继续阅读。

## 什么是速度{#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/)是一种基于Java的语言，专为模板和编写HTML内容脚本而设计。Marketo允许通过使用[脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)在电子邮件的上下文中使用它。 除其他外，这允许访问自定义对象中存储的数据。

您可以引用直接连接到潜在客户或联系人的父级和子级自定义对象，但不能引用第三级自定义对象。 对于每个自定义对象，每个人/联系人的10个最近更新的记录在运行时可用，并按从最近更新(0)到最旧更新(9)的顺序排列。

## 如何更改限制{#how-to-change-the-limit}

1. 转至&#x200B;**Admin**&#x200B;部分。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 单击&#x200B;**电子邮件**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在“自定义对象检索限制”表中，输入新的父检索限制，然后单击&#x200B;**保存更改**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>父检索限制值必须在10 - 100范围内。 子检索限制将自动设置给您。 这是通过将1000除以父检索限制来实现的。 例如，如果将“父项限制”设置为50，则“子项限制”将变为20(1000÷ 50 = 20)。

真贴心！ 现在，您可以从Velocity脚本访问更多自定义对象。
