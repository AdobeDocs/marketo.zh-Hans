---
unique-page-id: 2360309
description: 了解工作区和人员分区 — Marketo文档 — 产品文档
title: 了解工作区和人员分区
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 91b6460bf0fa7fed85d48887ec38203f2ee7440f
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# 了解工作区和人员分区 {#understanding-workspaces-and-person-partitions}

## 工作区 {#workspaces}

>[!CAUTION]
>
>工作区可能设置得比较复杂。 联系人 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 看看他们是否适合你。

工作区是Marketo中单独的区域，其中包含营销资源，如项目、登陆页面、电子邮件等。 它们可以由多人使用。 每个用户都有权访问一个或多个工作区。

>[!NOTE]
>
>**示例**
>
>您可能使用工作区的某些原因：
>
>* 地理位置：欧洲、亚洲和北美市场部均分配工作区
>* 业务单元： [!DNL Quicken]， [!DNL Quickbooks] 和 [!DNL TurboTax] 每个站点都有一个工作区
>
>在每种情况下，之所以进行分离，是因为营销资产完全不同。 如果他们共享营销资产，则工作区可能不是适合您的工具。

>[!NOTE]
>
>了解如何创建 [创建新工作区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## 跨工作区共享 {#sharing-across-workspaces}

以下是如何在工作区之间共享资源的。 它的工作方式与您要共享的任何内容相同；此示例显示了分段。

>[!NOTE]
>
>包含您的资产的父文件夹是唯一可共享的文件夹，而不是子文件夹。

1. 单击 **[!UICONTROL 数据库]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. 右键单击Segmentation文件夹，然后单击 **[!UICONTROL 新建文件夹]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. 命名文件夹并单击 **[!UICONTROL 创建]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. 将要共享的资产移动到文件夹中。

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. 右键单击文件夹，然后选择 **[!UICONTROL 共享文件夹]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. 选择要与共享文件夹的工作区，然后单击 **[!UICONTROL 保存]**. “共享文件夹”对话框将仅显示您具有查看权限的工作区。

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >现在，原始文件夹将有一个小绿色箭头，指示该文件夹已共享。 在共享的工作区中，文件夹将具有挂锁，表示只读。

可在多个工作区之间共享这些项目。

* 电子邮件模板
* 登陆页面模板
* 模型
* 智能营销活动
* [智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [分段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 代码片段

## 跨工作区克隆 {#cloning-across-workspaces}

对于不是模板的资源，最好在项目内将它们克隆为本地资源。 通过适当的访问级别，您可以将这些资产拖放到另一个工作区中：

* 程序
* 电子邮件
* 登陆页面
* Forms

>[!IMPORTANT]
>
>虽然上面列出的所有项目都可以跨工作区、电子邮件、表单和登陆页面进行克隆 _必须位于项目内_ 在克隆时。

>[!NOTE]
>
>克隆具有模板的资产时，必须与目标工作区共享这些模板。

## 将资产移到其他工作区 {#moving-assets-to-other-workspaces}

要将资源移动到新工作区，请将它们放入文件夹中，并将该文件夹拖到其他工作区中。

>[!NOTE]
>
>不能将包含成员的程序从一个工作区移动到另一个工作区。

## 人员分区 {#person-partitions}

人员分区就像单独的数据库。 每个分区都有各自的人员，他们不会执行重复数据删除或与其他分区混合。 如果您认为您的业务用例可能需要具有相同电子邮件地址的重复记录，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

您可以将人员分区分配给  [工作区](create-a-new-workspace.md) 在下列配置中：

* 一个工作区对一个人分区(1:1)
* 一个工作区对多个人员分区(1：x)
* 多个工作区到一人分区(x：1)

>[!NOTE]
>
>使用人员分区的原因：
>
>* 您的工作区不仅有不同的资源，而且还未共享任何人员
>* 由于其他业务原因需要重复项

>[!CAUTION]
>
>人员分区不会相互进行交互，因此进行设置时请务必谨慎。

>[!NOTE]
>
>了解如何 [创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
