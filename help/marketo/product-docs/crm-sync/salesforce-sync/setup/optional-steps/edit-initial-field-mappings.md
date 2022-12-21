---
unique-page-id: 4719287
description: 编辑初始字段映射 — Marketo文档 — 产品文档
title: 编辑初始字段映射
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 编辑初始字段映射 {#edit-initial-field-mappings}

>[!NOTE]
>
>此功能仅在初始同步到Salesforce之前可访问！ 一旦 **立即同步** 按钮，此操作将无法再完成。

在初始同步到Salesforce期间，Marketo会自动将名称类似的自定义字段合并到Marketo端的单个字段中，以确保可以与CRM中的Lead和Contact对象交换数据。 本文介绍如何自定义这些映射。

## 映射未映射的字段 {#map-unmapped-fields}

如果在“未映射的字段”文件夹中看到字段，则表示该字段未映射到Salesforce中潜在客户或联系人上的类似字段。 你可以解决。

1. 单击 **编辑映射**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. 打开 **未映射的自定义字段** 文件夹。

   ![](assets/two.png)

1. 将一个未映射的自定义字段拖动到另一个字段上，以将它们映射到一起。

   >[!NOTE]
   >
   >您只能编辑自定义字段映射。 无法修改标准字段映射。

   ![](assets/three.png)

1. 单击 **完成映射** 等你完成。

   ![](assets/four.png)

## 中断现有映射 {#break-existing-mapping}

如果您在潜在客户和联系人对象上具有名称相似的字段，Marketo会自动将它们映射到一起。 您可能会认为它们不同，并保存不同的数据。 像这样中断映射。

1. 单击 **编辑映射**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. 突出显示映射的字段，然后单击 **中断映射** 来分隔字段。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 单击 **完成映射** 等你完成。

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   不错！ 您几乎完成了初始同步。

## 重置架构 {#reset-schema}

1. 如果在处理映射时对Salesforce中的架构进行了一些更改，则可以通过单击 **重置架构**.

   * 所有映射更改都将重置！
   * 重置架构将只添加字段，而不会删除（即使您对同步用户隐藏了这些字段）。
   ![](assets/image2014-12-9-13-3a32-3a8.png)
