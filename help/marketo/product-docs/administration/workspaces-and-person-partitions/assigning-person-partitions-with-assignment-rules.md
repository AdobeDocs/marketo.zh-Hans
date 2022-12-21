---
unique-page-id: 2360327
description: 使用分配规则分配人员分区 — Marketo文档 — 产品文档
title: 使用分配规则分配人员分区
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# 使用分配规则分配人员分区 {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>[创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

使用人员分区时，请设置分配规则，将从CRM创建的人员路由到其各自的分区。

>[!NOTE]
>
>只有通过CRM和SOAP API在Marketo中创建的人员才会应用分配规则。

1. 在“管理员”下，单击“工作区和分区”。

   ![](assets/image2014-9-17-10-3a32-3a55.png)

1. 在 **人员分区** ，单击 **分配规则**.

   ![](assets/two-6.png)

1. 单击 **添加选择** 添加将人员路由到人员分区的条件。

   ![](assets/three-6.png)

1. 选择应基于条件的字段。

   ![](assets/four-5.png)

1. 选择选择运算符并输入一个值。

   ![](assets/five-1.png)

1. 选择您希望符合条件的人员进入的人员分区。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >您可以添加所需数量的选项。

1. 单击 **保存**.

   ![](assets/seven.png)

就这样！ 您为人员分区分配了用户填充规则！

>[!NOTE]
>
>如果不满足以前的任何条件，则将应用默认选择。
