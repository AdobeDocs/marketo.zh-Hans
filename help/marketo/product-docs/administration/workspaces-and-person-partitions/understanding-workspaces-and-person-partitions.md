---
unique-page-id: 2360309
description: 了解工作区和人员分区- Marketo Docs —— 产品文档
title: 了解工作区和人员分区
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# 了解工作区和人员分区 {#understanding-workspaces-and-person-partitions}

## 工作区 {#workspaces}

>[!CAUTION]
>
>工作区设置可能比较复杂。  联 [系Market](http://support.marketo.com/) Support，了解他们是否适合您。

工作区是Marketo中单独的区域，它们存放项目、登陆页、电子邮件等营销资产。 它们可供多人使用。 每个用户都有权访问一个或多个工作区。

>[!NOTE]
>
>**示例**
>
>您使用工作区的一些原因：
>
>* 地理位置：欧洲、亚洲和北美市场营销部门均可
>* 业务部门：Quicken、Quickbook和TurboTax均可获得工作区

>
>
在每种情况下，分离的原因是营销资产完全不同。 如果共享营销资产，那么工作区可能不适合您。

>[!NOTE]
>
>**深潜**
>
>了解如何创 [建新工作区](create-a-new-workspace.md)。

## 跨工作区共享 {#sharing-across-workspaces}

下面介绍如何在工作区之间共享资源。 它适用于您想要分享的任何内容；此示例显示分段。

>[!NOTE]
>
>包含您的资产的父级文件夹是唯一可共享的文件夹，而不是子级文件夹。

1. 创建新文件夹。

   ![](assets/one.png)

1. 命名要共享的文件夹。

   ![](assets/two.png)

1. 将要共享的资产移入文件夹。

   ![](assets/three.png)

1. 右键单击文件夹，然后选择“共 **享文件夹”**。

   ![](assets/four.png)

1. 选择要与其共享文件夹的工作区，然后单击“保 **存”**。 “共享文件夹”对话框将仅显示您具有视图权限的工作区。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >原始文件夹现在将显示一个绿色箭头，表示已共享。 在共享的工作区中，文件夹将具有挂锁，表示为只读。

您可以跨工作区共享这些项目。

* 电子邮件模板
* 登陆页模板
* 模型
* 智能活动
* [智能列表](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [细分](share-segmentations-across-workspaces-and-partitions.md)
* 代码片段

## 跨工作区克隆 {#cloning-across-workspaces}

对于非模板的资源，最好将它们克隆为项目内的本地资源。  通过适当的访问级别，您可以将这些资产拖放到另一个工作区中：

* 项目
* 电子邮件
* 登陆页
* Forms

>[!NOTE]
>
>克隆具有模板的资源时，这些模板必须与目标工作区共享。

## 将资产移至其他工作区 {#moving-assets-to-other-workspaces}

要将资产移到新工作区，请将其放入文件夹，然后将该文件夹拖动到另一个工作区。

>[!NOTE]
>
>无法将包含成员的项目从一个工作区移动到另一个工作区。

## 人员分区 {#person-partitions}

人员分区的操作方式与单独的数据库类似。 每个分区都有自己的人员，他们不会与其他分区进行重复数据消除或混合。 如果您认为您有业务使用案例，可能需要拥有具有相同电子邮件地址的重复记录，请与营销人员 [支持部门联系](http://support.marketo.com)。

您可以按照以下配置将人员 [分区](create-a-new-workspace.md) 分配到工作区：

* 一个工作区到一个人分区(1:1)
* 一个工作区到多个人员分区(1:x)
* 多个工作区到一个人分区(x:1)

>[!NOTE]
>
>**示例**
>
>您使用人员分区的原因：
>
>* 您的工作区不仅具有不同的资源，而且不共享任何人
>* 您希望重复出于其他业务原因

>



>[!CAUTION]
>
>人员分区之间不相互交互，因此在设置分区时要小心。

>[!NOTE]
>
>**深潜**
>
> 了解如何 [创建人员分区](create-a-person-partition.md)。

