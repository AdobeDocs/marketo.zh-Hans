---
unique-page-id: 4719287
description: 编辑初始字段映射 — Marketo文档 — 产品文档
title: 编辑初始字段映射
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 编辑初始字段映射 {#edit-initial-field-mappings}

>[!NOTE]
>
>此功能仅在初次同步到Salesforce之前才可访问。 一旦 **[!UICONTROL 立即同步]** 按钮时，无法再执行此操作。

在首次同步到Salesforce期间，Marketo Engage会自动将名称类似的自定义字段组合到Marketo端的单个字段中，以确保数据可以与CRM中的Lead和Contact对象交换。 本文介绍如何自定义这些映射。

## 映射未映射的字段 {#map-unmapped-fields}

当您在中看到字段 [!UICONTROL 未映射字段] 文件夹，这意味着它未映射到Salesforce中的Lead或Contact上的类似字段。 你可以解决的。

1. 单击 **[!UICONTROL 编辑映射]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. 打开 **[!UICONTROL 未映射的自定义字段]** 文件夹。

   ![](assets/two.png)

1. 将一个未映射的自定义字段拖到另一个上以将它们映射到一起。

   >[!NOTE]
   >
   >您只能编辑自定义字段映射。 无法修改标准字段映射。

   ![](assets/three.png)

1. 单击 **[!UICONTROL 完成映射]** 完成时。

   ![](assets/four.png)

## 中断现有映射 {#break-existing-mapping}

如果您在潜在客户和联系人对象中具有名称相似的字段，Marketo会自动将它们映射到一起。 您可能会认为它们是不同的并包含不同的数据。 像这样中断映射。

1. 单击 **[!UICONTROL 编辑映射]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. 突出显示映射的字段并单击 **[!UICONTROL 中断映射]** 以分隔字段。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 单击 **[!UICONTROL 完成映射]** 等你完事了。

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   太好了！ 初始同步即将完成。

## 重置架构 {#reset-schema}

1. 如果在处理映射时对Salesforce中的架构进行了一些更改，则可以通过单击 **[!UICONTROL 重置架构]**.

   * 将重置所有映射更改！
   * 重置架构只会添加字段，而不会删除字段（即使您对同步用户隐藏了字段）。

   ![](assets/image2014-12-9-13-3a32-3a8.png)
