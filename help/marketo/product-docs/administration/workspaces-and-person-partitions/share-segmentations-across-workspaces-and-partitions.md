---
unique-page-id: 7515767
description: 跨工作区和分区共享分段- Marketo Docs —— 产品文档
title: 跨工作区和分区共享分段
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# 跨工作区和分区共享分段 {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>本文仅针对具有工作区和分区的客户

## 什么是细分？ {#whats-a-segmentation}

Marketo擅长为项目或智能活动挑选合适的人。 但是，对于更永久的角色，您应使用细分。 他们需要在Marketo中使用高级动态内容。

>[!NOTE]
>
>**深潜**
>
>了 [解如何创建细分](../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)。

设置这些角色(**并使** 用工作区)后，您将希望在工作区中共享它们。 以下是一些值得了解的好事：

## 规则和提示 {#rules-tips}

* 每个营销订阅在多个工作区（不是每个工作区20个）中最多可包含20个“**总分段”**。
* 您只能与您有权访问的工作区共享分段。
* 确保创建并利用可见 **到所有分区的默认工作区**。

* 分段处理仅在创建分段的工作区中的人员上运行。

   * 创建要在默认工作区内共享的分段。

      * 批准分段
      * 共享工作区会看到锁定的文件夹，且分段为只读。
      * 无法编辑共享版本。 您只能编辑创建原始分段的位置。
   * 当您单击共享分段中的区段（例如医疗保健）时，您看到的人员将仅是分区中与您正在查看的工作区关联的人员。

      * 如果您在Workspace 1(WS1)中创建分段并与WS2共享，并且WS1无权访问WS2的分区，它将不会重新计算分段。
      * 如果您在具有有限分区的工作区中创建分段，然后与另一个工作区共享分段，则接收共享分段的工作区将仅在人员重叠时才会看到人员。


>[!NOTE]
>
>这些规则中有些有些复杂。 最简单的入门方法是测试特定人员。 您始终可以进行新细分并删除旧细分。

## 示例方案 {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

** ![](assets/image2015-5-27-16-3a26-3a48.png)

**

## 共享分段 {#share-a-segmentation}

1. 转到数据库。

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. 右键单击“区段”，然后选择“新建文件夹”。

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. 命名要在工作区间共享的文件夹(示例：共享细分。)

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. 将要共享的分段移入文件夹。

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. 右键单击文件夹，然后选择“共享文件夹”。

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. 选择要与之共享文件夹的工作区。 单击“保存”。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >该对话框显示您有权视图的工作区，这就是Marketo建议从默认工作区创建和共享区段的原因，默认工作区可以查看所有工作区和分区。

始发文件夹显示在数据库树中，其中带有一个箭头，指示已与其他工作区共享该文件夹。 在共享工作区中，文件夹会显示一个锁，指示已从其他工作区共享文件夹的内容且为只读。

>[!NOTE]
>
>**相关文章**
>
>[分段和片段](http://docs.marketo.com/display/docs/segmentation+and+snippets)

