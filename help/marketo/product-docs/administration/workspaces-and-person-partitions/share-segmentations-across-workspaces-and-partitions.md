---
unique-page-id: 7515767
description: 跨工作区和分区共享细分 — Marketo Docs — 产品文档
title: 跨工作区和分区共享分段
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 跨工作区和分区共享分段{#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>本文仅针对具有工作区和分区的客户。

## 什么是细分？{#whats-a-segmentation}

Marketo擅长为项目或智能活动挑选合适的人。 但是，对于更加永久性的角色，您应使用细分。 他们需要在Marketo中使用高级动态内容。

>[!NOTE]
>
>了解[如何创建区段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)。

设置这些角色后（_和_&#x200B;您使用工作区），您将希望在工作区之间共享它们。 以下是一些值得了解的好事：

## 规则和提示{#rules-tips}

* 每个Marketo订阅可在多个工作区中最多包含20个“总计”区段（**不是每个工作区** 20个）。
* 您只能与您有权访问的工作区共享分段。
* 确保创建并利用&#x200B;**默认工作区，该工作区可以查看所有分区**。

* 分段处理仅在创建分段的工作区中的人员上运行。

   * 在默认工作区中创建要共享的分段。
      * 批准分段
      * 共享工作区会看到锁定的文件夹，而分段为只读。
      * 无法编辑共享版本。 您只能编辑创建原始分段的位置。
   * 当您单击共享分段中的区段（例如医疗保健）时，您看到的人将仅是分区中与您查看的工作区关联的人员。
      * 如果您在Workspace 1(WS1)中创建分段并与WS2共享，且WS1无权访问WS2的分区，它将不会重新计算分段。
      * 如果您在具有有限分区的工作区中创建分段，然后与另一个工作区共享，则接收共享分段的工作区将仅在人员重叠时才会看到他们。


>[!NOTE]
>
>其中一些规则有点复杂。 最简单的入门方法是测试特定人员。 您始终可以进行新细分并删除旧细分。

## 示例方案{#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## 共享分段{#share-a-segmentation}

1. 转到&#x200B;**Database**。

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. 右键单击&#x200B;**分段**&#x200B;并选择&#x200B;**新建文件夹**。

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. 命名要跨工作区共享的文件夹(示例：共享细分)。

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. 将要共享的分段移入文件夹。

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. 右键单击文件夹，然后选择&#x200B;**共享文件夹**。

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. 选择要与其共享文件夹的工作区。 单击&#x200B;**保存**。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >该对话框显示您有权视图的工作区，这就是为什么Marketo建议从可查看所有工作区和分区的“默认”工作区创建和共享区段。

始发文件夹显示在“数据库”树中，并带有一个箭头，指示已与其他工作区共享。 从共享工作区中，文件夹会显示一个锁，指示已从其他工作区共享文件夹的内容且为只读。
