---
unique-page-id: 2360327
description: 使用分配规则分配人员分区 — Marketo文档 — 产品文档
title: 使用分配规则分配人员分区
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# 使用分配规则分配人员分区 {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>[创建人员分区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

使用人员分区时，请设置分配规则，以将从CRM创建的人员路由到其各自的分区。

>[!NOTE]
>
>只有在Marketo中通过SOAP API从CRM创建的人员才会应用分配规则。

1. 转到&#x200B;**[!UICONTROL 管理员]**&#x200B;区域。

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. 单击&#x200B;**[!UICONTROL 工作区和分区]**。

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. 在&#x200B;**[!UICONTROL 人员分区]**&#x200B;选项卡下，单击&#x200B;**[!UICONTROL 分配规则]**。

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. 单击&#x200B;**[!UICONTROL 添加选择]**&#x200B;可添加将人员路由到人员分区的条件。

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. 选择条件应基于的字段。

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. 选择选择运算符并输入值。

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. 选择您希望满足条件的人员所属的人员分区。

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >您可以添加任意多个选项。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

你拿到了！ 您已分配了用于向人员分区填充人员的规则！

>[!NOTE]
>
>如果不满足先前的任何条件，则将应用默认选择。
