---
unique-page-id: 2360309
description: 了解工作区和人员分区 — Marketo Docs — 产品文档
title: 了解工作区和人员分区
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 了解工作区和人员分区{#understanding-workspaces-and-person-partitions}

## 工作区{#workspaces}

>[!CAUTION]
>
>工作区设置可能很复杂。 请联系[Marketo支持部门](https://nation.marketo.com/t5/Support/ct-p/Support)，了解他们是否适合您。

工作区是Marketo中存放项目、登陆页、电子邮件等营销资产的独立区域。 它们可以被多个人使用。 每个用户都可以访问一个或多个工作区。

>[!NOTE]
>
>**示例**
>
>您使用工作区的一些原因：
>
>* 地理位置：欧洲、亚洲和北美的营销部门均可获得工作区
>* 业务单位：Quicken、Quickbook和TurboTax每个都能获得工作区

>
>
在每种情况下，分离都是因为营销资产完全不同。 如果共享营销资产，则工作区可能不是适合您的工具。

>[!NOTE]
>
>了解如何创建[新工作区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md)。

## 跨工作区共享{#sharing-across-workspaces}

下面介绍如何跨工作区共享资产。 对于您想要分享的任何内容，它都能起到同样的作用；此示例显示分段。

>[!NOTE]
>
>只有包含您的资产的父文件夹才能共享，而子文件夹不能共享。

1. 创建新文件夹。

   ![](assets/one.png)

1. 命名要共享的文件夹。

   ![](assets/two.png)

1. 将要共享的资产移动到文件夹中。

   ![](assets/three.png)

1. 右键单击文件夹，然后选择&#x200B;**共享文件夹**。

   ![](assets/four.png)

1. 选择要与其共享文件夹的工作区，然后单击&#x200B;**保存**。 “共享文件夹”对话框将仅显示您有权视图的工作区。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >原始文件夹现在将显示一个绿色箭头，表示已共享。 在共享的工作区中，文件夹将具有挂锁图标（表示只读）。

您可以跨工作区共享这些项目。

* 电子邮件模板
* 登陆页模板
* 模型
* 智能活动
* [智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [细分](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 片段

## 跨工作区克隆{#cloning-across-workspaces}

对于非模板的资源，最好将它们克隆为项目内的本地资源。  通过适当的访问级别，您可以将这些资产拖放到另一个工作区中：

* 项目
* 电子邮件
* 登陆页
* Forms

>[!NOTE]
>
>克隆具有模板的资源时，必须与目标工作区共享这些模板。

## 将资产移至其他工作区{#moving-assets-to-other-workspaces}

要将资产移到新工作区，请将其放入一个文件夹，然后将该文件夹拖动到另一个工作区。

>[!NOTE]
>
>不能将包含成员的项目从一个工作区移动到另一个工作区。

## 人员分区{#person-partitions}

人员分区的作用类似于单独的数据库。 每个分区都有其自己的人员，他们不会与其他分区进行重复数据消除或混合。 如果您认为您有业务用例，而且可能需要具有具有相同电子邮件地址的重复记录，请联系[Marketo支持部门](https://nation.marketo.com/t5/Support/ct-p/Support)。

您可以按照以下配置将人员分区分配给[workspaces](create-a-new-workspace.md):

* 一个工作区到一个人分区(1:1)
* 一个工作区到多个人分区(1:x)
* 多个工作区(x:1)

>[!NOTE]
>
>您使用人员分区的原因：
>
>* 您的工作区不仅具有不同的资源，而且不共享任何人
>* 您希望重复出于其他业务原因


>[!CAUTION]
>
>人分区不会相互交互，因此在设置它们时要小心。

>[!NOTE]
>
>了解如何[创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)。
