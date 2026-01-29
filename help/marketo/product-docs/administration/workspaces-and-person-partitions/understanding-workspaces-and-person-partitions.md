---
unique-page-id: 2360309
description: 了解工作区与人员分区 — Marketo 文档 — 产品文档
title: 了解工作区和人员分区
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '528'
ht-degree: 100%

---

# 了解工作区和人员分区 {#understanding-workspaces-and-person-partitions}

## 工作区 {#workspaces}

>[!CAUTION]
>
>工作区的设置可能较为复杂。请联系 [Marketo 支持](https://nation.marketo.com/t5/Support/ct-p/Support)，确认工作区是否适合您的使用场景。

工作区是 Marketo 中彼此独立的区域，用于存放项目、登陆页面、电子邮件等营销资源。工作区可供多位用户共同使用。每位用户可以访问一个或多个工作区。

>[!NOTE]
>
>**示例**
>
>您可能使用工作区的原因包括：
>
>* 地域：欧洲、亚洲和北美的营销团队各自使用独立的工作区
>* 业务单元：[!DNL Quicken]、[!DNL Quickbooks] 和 [!DNL TurboTax] 各自拥有独立的工作区
>
>在上述情况下，进行区分是因为各自使用的营销资源完全不同。如果需要共享营销资源，那么工作区可能并不适合您的需求。

>[!NOTE]
>
>了解如何[创建新的工作区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md)。

## 跨工作区共享 {#sharing-across-workspaces}

以下说明如何在不同工作区之间共享资源。该方法适用于所有可共享的内容；此示例以分段为例。

>[!NOTE]
>
>只能共享包含资源的父文件夹，不能共享其子文件夹。

1. 单击 **[!UICONTROL Database]**。

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. 右键点击“分段”文件夹，然后点击 **[!UICONTROL New Folder]**。

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. 为文件夹命名，然后点击 **[!UICONTROL Create]**。

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. 将需要共享的资源移动到该文件夹中。

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. 右键点击该文件夹，并选择 **[!UICONTROL Share Folder]**。

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. 选择要共享该文件夹的工作区，然后点击 **[!UICONTROL Save]**。“共享文件夹”对话框只会显示您有权限查看的工作区。

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >原始文件夹将显示一个小绿箭头，表示该文件夹已共享。在共享的工作区中，该文件夹将显示一个锁定图标，表示为只读。

以下项目可以在不同工作区之间共享。

* 电子邮件模板
* 登陆页面模板
* 模型
* 智能营销活动
* [智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [分段](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* 代码段

## 跨工作区克隆 {#cloning-across-workspaces}

对于非模板类资源，最佳做法是在项目中将其克隆为本地资源。在具备相应访问权限的情况下，您可以将以下资源拖放到另一个工作区中：

* 项目
* 电子邮件
* 登陆页面
* 表单

>[!IMPORTANT]
>
>虽然上述所有项目都可以跨工作区克隆，但电子邮件、表单和登陆页面在克隆时&#x200B;_必须位于某个项目中_。

>[!NOTE]
>
>在克隆包含模板的资源时，相关模板必须已共享给目标工作区。

## 将资源移动到其他工作区 {#moving-assets-to-other-workspaces}

要将资源移动到新的工作区，请先将其放入一个文件夹中，然后将该文件夹拖动到目标工作区。

>[!NOTE]
>
>无法将包含成员的项目从一个工作区移动到另一个工作区。

## 人员分区 {#person-partitions}

人员分区的作用类似于独立的数据库。每个分区都有自己独立的人员数据，不会与其他分区进行去重或混合。如果您的业务场景确实需要允许存在使用相同电子邮件地址的重复记录，请联系 [Marketo 支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

您可以按以下配置方式将人员分区分配给[工作区](create-a-new-workspace.md)：

* 一个工作区对应一个人员分区（1:1）
* 一个工作区对应多个人员分区（1:x）
* 多个工作区对应一个人员分区（x:1）

>[!NOTE]
>
>您可能使用人员分区的原因包括：
>
>* 您的工作区不仅资源不同，而且人员数据也不共享
>* 出于其他业务原因，您需要允许存在重复记录

>[!CAUTION]
>
>人员分区彼此之间不会交互，因此在设置时需格外谨慎。

>[!NOTE]
>
>了解如何[创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)。
