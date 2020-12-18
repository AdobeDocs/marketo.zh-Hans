---
unique-page-id: 4718683
description: 批准阶段并将潜在客户分配到收入模型- Marketo Docs —— 产品文档
title: 批准阶段并将潜在客户分配给收入模型
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# 批准阶段并将销售线索分配给收入模型{#approving-stages-and-assigning-leads-to-a-revenue-model}

通过添加现有潜在客户并为任何新潜在客户创建分配规则，使您的&#x200B;**收入** **模型**&#x200B;启动并运行。

## 批准阶段{#approving-stages}

在添加任何潜在客户之前，让我们批准您模型的各个阶段。

1. 转至**Analytics **区域。** **

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. 选择要批准其舞台的模型。

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. 在&#x200B;**模型操作**&#x200B;下，选择&#x200B;**批准** **阶段**。

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. 你会收到警报；单击&#x200B;**分配潜在客户**。

   ![](assets/image2015-4-28-17-3a5-3a39.png)

太棒了！ 让我们继续分配这些潜在客户。

## 分配现有潜在客户{#assigning-existing-leads}

[创建智能列](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 表，以在潜在客户数据库中标识模型的一个阶段的潜在客户。

1. 创建[智能列表](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)后，单击&#x200B;**潜在客户**&#x200B;选项卡。

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. 单击&#x200B;**全选**&#x200B;以选择Lead。

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. 打开&#x200B;**潜在客户操作**&#x200B;下拉框，然后选择&#x200B;**特殊**。 单击&#x200B;**更改收入阶段**。

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. 选择正确的&#x200B;**Model**&#x200B;和正确的&#x200B;**Stage**。 单击&#x200B;**立即运行**。

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. 重复上述步骤，直到将所有潜在客户分配给模型的各个阶段。

太好了！ 要指定如何将新潜在客户分配给阶段，请创建分配规则。

>[!NOTE]
>
>如果您的模型处于“已批准的阶段”状态，您将不会在潜在客户的事件日志中看到任何“更改收入阶段”活动。 如果您的模型已获得完全批准，则如果将潜在客户移动到当前所在的同一阶段，将跳过此流步骤。

## 新潜在客户：创建分配规则{#new-leads-create-assignment-rules}

1. 再次单击** Marketo Home**，然后选择&#x200B;**Analytics**。

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. `Click your model in the tree, then the`**`Model Actions`**`menu, selecting`**`Assignment Rules`** `.`

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. `If your assignment rules contain more than just one default choice click **Stage, **make your selection, then click`**`Add Choice`**`.`

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## 分配规则示例{#example-assignment-rule}

创建“潜在客户得分”规则，以将具有最低得分的新潜在客户分配给相应的步骤。

1. 在&#x200B;**If**&#x200B;下，选择&#x200B;**潜在客户得分**。 然后，至少选择&#x200B;****。
“ ![](assets/image2015-4-29-13-3a27-3a8.png)

   “

1. 在字段中输入&#x200B;**40**&#x200B;并选择&#x200B;**销售线索**&#x200B;作为阶段。 单击&#x200B;**保存**&#x200B;以完成。

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>要批准您的模型，请阅读我们的帮助页面，网址为** [批准和取消批准收入模型](approve-unapprove-a-revenue-model.md)**。

