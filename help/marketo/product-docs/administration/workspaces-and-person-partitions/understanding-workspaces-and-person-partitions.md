---
unique-page-id: 2360309
description: 了解工作区和人员分区 — Marketo文档 — 产品文档
title: 了解工作区和人员分区
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 了解工作区和人员分区 {#understanding-workspaces-and-person-partitions}

## 工作区 {#workspaces}

>[!CAUTION]
>
>工作区的设置可能会非常复杂。 联系人 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 来查明他们是否适合你。

工作区是Marketo中单独的区域，用于存放项目、登陆页面、电子邮件等营销资产。 它们可供多个人使用。 每个用户都有权访问一个或多个工作区。

>[!NOTE]
>
>**示例**
>
>使用工作区的一些原因：
>
>* 地理位置：欧洲、亚洲和北美的营销部门均可获得工作区
>* 业务部门：Quicken、Quickbook和TurboTax每个人都有一个工作区
>
>在每种情况下，区分都是因为营销资产完全不同。 如果他们共享营销资产，则工作区可能不适合您。

>[!NOTE]
>
>了解如何创建 [创建新工作区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## 跨工作区共享 {#sharing-across-workspaces}

以下是如何在工作区之间共享资产。 它对于您想分享的任何内容都是一样的；此示例显示区段。

>[!NOTE]
>
>只有包含您的资产的父文件夹才能共享，而不能共享子文件夹。

1. 创建新文件夹。

   ![](assets/one.png)

1. 命名要共享的文件夹。

   ![](assets/two.png)

1. 将要共享的资产移入文件夹。

   ![](assets/three.png)

1. 右键单击文件夹并选择 **共享文件夹**.

   ![](assets/four.png)

1. 选择要与其共享文件夹的工作区，然后单击 **保存**. “共享文件夹”对话框将仅显示您有权查看的工作区。

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >原始文件夹现在将有一个绿色的小箭头，表示已共享该文件夹。 在共享的工作区中，文件夹将具有挂锁图标，表示为只读。

您可以跨工作区共享这些项目。

* 电子邮件模板
* 登陆页面模板
* 模型
* 智能营销活动
* [智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [分段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 代码片段

## 跨工作区克隆 {#cloning-across-workspaces}

对于不是模板的资产，最好将它们克隆为程序内的本地资产。  通过适当的访问级别，您可以将这些资产拖放到另一个工作区中：

* 程序
* 电子邮件
* 登陆页面
* Forms

>[!NOTE]
>
>克隆具有模板的资产时，必须与目标工作区共享这些模板。

## 将资产移动到其他工作区 {#moving-assets-to-other-workspaces}

要将资产移动到新工作区，请将资产放入文件夹中，然后将该文件夹拖动到另一个工作区。

>[!NOTE]
>
>无法将包含成员的项目从一个工作区移动到另一个工作区。

## 人员分区 {#person-partitions}

人员分区的操作类似于单独的数据库。 每个分区都有其自己的人员，他们不会消除重复数据或与其他分区混合使用。 如果您认为有业务用例需要具有具有相同电子邮件地址的重复记录，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

您可以将人员分区分配到  [工作区](create-a-new-workspace.md) 在以下配置中：

* 一个工作区到一个人员分区(1:1)
* 一个工作区到多个人员分区(1:x)
* 多个工作区对应一个人员分区(x:1)

>[!NOTE]
>
>使用人员分区的原因：
>
>* 您的工作区不仅具有不同的资产，而且不会共享任何人员
>* 出于其他业务原因，您需要重复项


>[!CAUTION]
>
>人员分区不会相互交互，因此在设置时要小心。

>[!NOTE]
>
>了解如何 [创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
