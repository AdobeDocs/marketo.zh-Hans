---
unique-page-id: 2360327
description: 使用分配规则分配人员分区- Marketo文档——产品文档
title: 使用分配规则分配人员分区
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
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
>* [创建人员分区](create-a-person-partition.md)

>



使用人员分区时，请设置分配规则，将从您的CRM创建的人员路由到其各自的分区。

>[!NOTE]
>
>只有在Marketo中通过CRM和SOAP API创建的人员才会应用分配规则。

1. 在“管理员”下，单击“工作区和分区”。

![](assets/image2014-9-17-10-3a32-3a55.png)

1. 在“**人员分区**”选项卡下，单击“分配 **规则”**。

   ![](assets/two-6.png)

1. 单击**添加选项**，为人员路由添加条件。

   ![](assets/three-6.png)

1. 选择应基于条件的字段。

   ![](assets/four-5.png)

1. 选择选择运算符并输入值。
1. ![](assets/five-1.png)

1. 选择您希望符合条件的人员进入的人员分区。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >
   >您可以添加任意所需数量的选项。

   单击“保存”。
   ![](assets/seven.png)

你拿到了！ 您已经为人员分区分配了规则！

>[!NOTE]
>
>如果未满足以前的条件，则将应用默认选择。

