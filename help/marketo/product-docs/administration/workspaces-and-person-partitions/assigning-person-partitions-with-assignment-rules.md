---
unique-page-id: 2360327
description: 使用分配规则分配人员分区 — Marketo文档 — 产品文档
title: 使用分配规则分配人员分区
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
source-git-commit: 57b94e643154b1463d9fd65295a66f1a3286fd40
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---

# 使用分配规则分配人员分区 {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>[创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

使用人员分区时，请设置分配规则以将从CRM创建的人员路由到其各自的分区。

>[!NOTE]
>
>只有在Marketo中通过CRM和SOAP API创建的人员才会应用分配规则。

1. 转到 **管理员** 区域。

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. 单击 **工作区和分区**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. 在 **人员分区** 选项卡，单击 **分配规则**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. 单击 **添加选项** 添加将人员路由到人员分区的条件。

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. 选择条件应基于的字段。

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. 选择选择运算符并输入值。

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. 选择您希望符合条件的人员归入的人员分区。

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >您可以添加任意多个选项。

1. 单击 **保存**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

你拿到了！ 您已经分配了使用人员填充人员分区的规则！

>[!NOTE]
>
>如果不满足以前的任何条件，则将应用默认选择。
