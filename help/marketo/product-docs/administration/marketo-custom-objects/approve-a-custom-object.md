---
unique-page-id: 10094188
description: 批准自定义对象- Marketo Docs —— 产品文档
title: 批准自定义对象
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# 批准自定义对象 {#approve-a-custom-object}

必须批准自定义对象，然后才能使用它。 对于新的自定义对象和您编辑的自定义对象，该过程略有不同。

## 批准新的自定义对象 {#approve-a-new-custom-object}

您创建了全新的自定义对象。 下面介绍如何批准它。

1. 在“管理员” **中，单击“营销** ”“自定义对象”，然后选择处于“草稿”状态的对象。

   ![](assets/one.png)

1. 单击“自 **定义对象操作** ”下拉框，然后选 **择“批准对象”**。

   ![](assets/two.png)

1. 状态将变为“已批准”。

   ![](assets/three.png)

   >[!NOTE]
   >
   >在一对多结构中 *使用的自定义对象* ，必须至少具有一个重复数据消除字段、链接字段、链接对象名称和要批准的链接字段名称。
   >
   >
   >在多对多结 *构中使用的自定义对* 象在您批准时 **** ，不需要链接字段、链接对象名称或链接字段名称（因为它们位于中间对象中）。
   >
   >
   >用作中间对象的自 *定义对象* ，需要链接字段、链接对象名称和链接字段名称， **但不需要重复** 消除字段。
   >
   >
   >有关详 [细信息，请参阅了解Marketo](understanding-marketo-custom-objects.md) Custom Objects。

就这样！ 现在，您可以在过滤器和触发器的约束中选择要在活动中使用的自定义对象。

## 批准已编辑的自定义对象 {#approve-an-edited-custom-object}

编辑已批准的自定义对象后，必须批准草稿以将自定义对象返回到“已批准”状态。

1. 编辑已批准的自定义对象时，它将收到“已批准且已草稿”状态。

   ![](assets/four.png)

1. 准备好批准草稿时，单击“自定义对 **象操作** ”下拉框并选 **择批准对象**。

   ![](assets/five-1.png)

1. 预览显示草稿中更改的项目。 单击 **批准**。

   ![](assets/six-1.png)

