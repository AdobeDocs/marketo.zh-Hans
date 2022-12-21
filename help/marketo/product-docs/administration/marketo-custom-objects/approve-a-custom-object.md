---
unique-page-id: 10094188
description: 批准自定义对象 — Marketo文档 — 产品文档
title: 批准自定义对象
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# 批准自定义对象 {#approve-a-custom-object}

必须批准自定义对象，然后才能使用它。 对于新的自定义对象和您编辑的对象，该过程会略有不同。

## 批准新的自定义对象 {#approve-a-new-custom-object}

您已创建一个全新的自定义对象。 下面是如何批准它。

1. 在管理员中，单击 **Marketo自定义对象** 并选择处于“草稿”状态的对象。

   ![](assets/one.png)

1. 单击 **自定义对象操作** 下拉框并选择 **批准对象**.

   ![](assets/two.png)

1. 状态将更改为“已批准”。

   ![](assets/three.png)

   >[!NOTE]
   >
   >在 _一对多结构_ 必须至少具有一个重复数据删除字段、链接字段、链接对象名称和要批准的链接字段名称。
   >
   >在 _多对多结构_ **does&#39;t** 在您批准链接字段、链接的对象名称或链接的字段名称时，需要该字段名称（因为它们位于中间对象中）。
   >
   >用作 _中介对象_ 需要链接字段、链接的对象名称和链接的字段名称，但 **does&#39;t** 需要一个重复数据消除字段。
   >
   >请参阅 [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以了解更多信息。

就这样！ 现在，您可以在过滤器和触发器的约束中选择要在营销活动中使用的自定义对象。

## 批准编辑的自定义对象 {#approve-an-edited-custom-object}

编辑已批准的自定义对象后，必须批准草稿以将自定义对象返回到“已批准”状态。

1. 在编辑已批准的自定义对象时，该对象将收到“已批准且为草稿”状态。

   ![](assets/four.png)

1. 准备好批准草稿后，单击 **自定义对象操作** 下拉框并选择 **批准对象**.

   ![](assets/five-1.png)

1. 预览显示草稿中更改的项目。 单击 **批准**.

   ![](assets/six-1.png)
