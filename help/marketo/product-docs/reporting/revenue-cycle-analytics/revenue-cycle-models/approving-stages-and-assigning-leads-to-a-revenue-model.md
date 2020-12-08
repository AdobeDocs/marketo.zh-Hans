---
unique-page-id: 4718683
description: 批准阶段并将潜在客户分配到收入模型- Marketo Docs —— 产品文档
title: 批准阶段并将潜在客户分配给收入模型
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# 批准阶段并将潜在客户分配给收入模型 {#approving-stages-and-assigning-leads-to-a-revenue-model}

通过添 **加现** 有Lead **** ，为任何新Lead创建分配规则，来建立并运行您的收入模型。

## 批准阶段 {#approving-stages}

在添加任何潜在客户之前，让我们批准您模型的各个阶段。

1. 转到**Analytics区 **域。** **

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 选择要批准其舞台的模型。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. 在“模 **型操作**”下，选 **择“批****准阶段**”。

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 你会收到警报；单击“ **分配潜在客户**”。

   ![](assets/image2015-4-28-17-3a5-3a39.png)

太棒了！ 让我们继续分配这些潜在客户。

## 分配现有潜在客户 {#assigning-existing-leads}

[创建智能列表](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ，在潜在客户库中为模型的一个阶段确定潜在客户。

1. 创建智能 [列表后](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)，单击潜在 **客户选项卡** 。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 单击 **全选** ，以选择潜在客户。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. 打开“ **潜在客户操作** ”下拉框并选择 **“特殊”**。 单击 **更改收入阶段**。

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 选择正确的 **模型** 和正确的 **舞台**。 单击“ **立即运行**”。

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. 重复上述步骤，直到将所有潜在客户分配给模型的各个阶段。

太好了！ 要指定如何将新潜在客户分配给阶段，请创建分配规则。

>[!NOTE]
>
>如果您的模型处于“已批准的阶段”状态，您将不会在潜在客户的事件日志中看到任何“更改收入阶段”活动。 如果您的模型已获得完全批准，则如果将潜在客户移动到当前所在的同一阶段，将跳过此流步骤。

## 新潜在客户：创建分配规则  {#new-leads-create-assignment-rules}

1. 再次单击** Marketo主页**，然后选择“分 **析”**。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. `Click your model in the tree, then the`**`Model Actions`**`menu, selecting`**`Assignment Rules`** `.`

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. `If your assignment rules contain more than just one default choice click **Stage, **make your selection, then click`**`Add Choice`**`.`

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 分配规则示例 {#example-assignment-rule}

创建“潜在客户得分”规则，以将具有最低得分的新潜在客户分配给相应的步骤。

1. 在“如 **果**”下，选 **择潜在客户得分**。 然后至 **少选择**。“ ![](assets/image2015-4-29-13-3a27-3a8.png)

   `

1. 在字 **段中** 输入40，然后选择 **销售潜在客** 户作为“阶段”。 单击 **保存** 以完成。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!NOTE]
>
>**相关文章**
>
>要批准您的模型，请阅读我们的帮助页面** [批准和取消批准收入模型](approve-unapprove-a-revenue-model.md)**。

