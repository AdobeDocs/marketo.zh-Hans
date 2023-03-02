---
unique-page-id: 7515767
description: 跨工作区和分区共享分段 — Marketo文档 — 产品文档
title: 跨工作区和分区共享分段
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
source-git-commit: 4d4d87d2a03bc0966a6e77d97cb68a2c38a3c676
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 跨工作区和分区共享分段 {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>本文仅适用于拥有工作区和分区的客户。

## 什么是分段？ {#whats-a-segmentation}

Marketo擅长为项目或明智的营销活动挑选合适的人。 但是，对于更永久的角色，您应使用分段。 在Marketo中使用高级动态内容时需要这些权限。

>[!NOTE]
>
>了解 [如何创建分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

设置这些角色后(_和_ （例如，您使用工作区），您将在多个工作区中共享这些工作区。 以下是一些需要了解的好信息：

## 规则和提示 {#rules-tips}

* 每个Marketo订阅最多可以包含跨多个工作区的20个分段“总计”(**每个工作区不是20**)。
* 您只能与有权访问的工作区共享分段。
* 确保创建和利用 **对所有分区具有可见性的默认工作区**.

* 分段处理仅对创建分段的工作区中的人员运行。

   * 创建要在默认工作区中共享的分段。
      * 批准分段
      * 共享工作区将看到一个锁定的文件夹，并且分段为只读。
      * 无法编辑共享版本。 您只能编辑创建它的原始分段。
   * 单击共享区段中的区段（例如，医疗保健）时，您看到的人员将只是分区中与您查看的工作区相关联的人员。
      * 如果在Workspace 1 (WS1)中创建分段并与WS2共享，而WS1无权访问WS2的分区，则不会重新计算分段。
      * 如果在具有有限分区的工作区中创建分段，然后将其与另一个工作区共享，则接收共享分段的工作区将仅看到重叠的人员。


>[!NOTE]
>
>其中一些规则有点复杂。 最简单的入门方法是与特定人员一起进行测试。 您始终可以生成新的分段并删除旧的分段。

## 示例场景 {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

![](assets/image2015-5-27-16-3a26-3a48.png)

## 共享分段 {#share-a-segmentation}

1. 转到 **数据库**.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. 右键单击 **分段** 并选择 **新建文件夹**.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. 命名要在工作区之间共享的文件夹（例如：共享分段）。

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. 将要共享的分段移动到文件夹中。

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. 右键单击文件夹并选择 **共享文件夹**.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. 选择要与其共享文件夹的工作区。 单击 **保存**.

   ![](assets/share-segmentations-across-workspaces-and-partitions.png)

   >[!NOTE]
   >
   >该对话框显示您有权查看的工作区，因此Marketo建议从默认工作区创建和共享可看到所有工作区和分区的分段。

源文件夹显示在数据库树中，其箭头指示它与其他工作区共享。 在共享工作区中，文件夹显示时带有锁，表示文件夹的内容已从其他工作区共享，且为只读。
