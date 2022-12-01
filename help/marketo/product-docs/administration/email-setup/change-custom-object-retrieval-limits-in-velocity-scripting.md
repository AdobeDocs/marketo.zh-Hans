---
description: 在Velocity脚本中更改自定义对象检索限制 — Marketo文档 — 产品文档
title: Velocity脚本中自定义对象检索限制的变更
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Velocity脚本中自定义对象检索限制的变更 {#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用Velocity脚本在电子邮件中显示自定义对象数据，则此功能可能适合您。 默认情况下，允许您从Velocity脚本访问10个父自定义对象。 如果您需要访问更多，请阅读。

## 什么是Velocity {#what-is-velocity}

[Apache Velocity](https://velocity.apache.org/) 是一种基于Java构建的语言，专为模板和脚本HTML内容而设计。 Marketo允许通过使用 [脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). 此外，还允许访问自定义对象中存储的数据。

可以引用直接连接到潜在客户或联系人的父和子自定义对象，但不能引用第三级自定义对象。 对于每个自定义对象，每个人员/联系人的10条最近更新的记录在运行时可用，并按从最近更新(0)到最早更新(9)的顺序进行排序。

## 如何更改限制 {#how-to-change-the-limit}

1. 转到 **管理员** 中。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 单击 **电子邮件**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在“自定义对象检索限制”(Custom Object Retrieval Limits)表格中，输入新的父项检索限制并单击 **保存更改**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>父检索限制值必须在10 - 100范围内。 子检索限制将自动为您设置。 这是通过将1000除以父检索限制来完成的。 例如，如果将父项限制设置为50，则子项限制将变为20(1000÷ 50 = 20)。

真贴心！ 现在，您可以从Velocity脚本访问更多自定义对象。
