---
unique-page-id: 4719287
description: 编辑初始字段映射- Marketo Docs —— 产品文档
title: 编辑初始字段映射
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# 编辑初始字段映射{#edit-initial-field-mappings}

>[!NOTE]
>
>**提醒**
>
>此功能仅在初始同步到Salesforce之前才可访问！ 按下&#x200B;**Sync Now**&#x200B;按钮后，将无法再执行此操作。

在与Salesforce进行初始同步期间，Marketo会自动将名称相似的自定义字段合并到Marketo端的单个字段中，以确保可以与CRM中的Lead和Contact对象交换数据。 本文介绍如何自定义这些映射。

## 映射未映射字段{#map-unmapped-fields}

当您在未映射的字段文件夹中看到字段时，这意味着它未映射到Salesforce中潜在客户或联系人上的类似字段。 你可以解决。

1. 单击编辑映射。

![](assets/image2014-12-9-13-3a31-3a0.png)

1. 打开&#x200B;**未映射的自定义字段**&#x200B;文件夹。

   ![](assets/two.png)

1. 将一个未映射的自定义字段拖动到另一个字段上，以将它们映射到一起。

   >[!NOTE]
   >
   >只能编辑自定义字段映射。 无法修改标准字段映射。

   ![](assets/three.png)

1. 完成后，单击&#x200B;**完成映射**。

   ![](assets/four.png)

## 中断现有映射{#break-existing-mapping}

如果您在潜在客户和联系人对象上具有类似名称的字段，Marketo会自动将它们映射到一起。 您可能认为它们不同，并保留不同的数据。 像这样中断映射。

1. 单击&#x200B;**编辑映射**。

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. 高亮显示映射的字段，然后单击&#x200B;**中断映射**&#x200B;以分隔这些字段。

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. 完成后，单击&#x200B;**完成映射**。

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   不错！ 初始同步快完成了。

## 重置模式{#reset-schema}

1. 如果在处理映射时对Salesforce中的模式进行了一些更改，则可以单击&#x200B;**重置模式**&#x200B;来拉取这些更改。

   * 将重置所有映射更改！
   * 重置模式只会添加字段，而不会删除（即使您从同步用户中隐藏它们）。

   ![](assets/image2014-12-9-13-3a32-3a8.png)

