---
unique-page-id: 9438139
description: 将人员添加到阻止列表- Marketo文档 — 产品文档
title: 将人员添加到阻止列表
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# 将人员添加到阻止列表 {#add-person-to-blocklist}

将人员添加到您的阻止列表会阻止他们接收您的信件。

1. [创建新的默认程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) 并命名它 **添加到阻止列表**.

1. 单击 **新建** 并选择 **新建本地资产**.

   ![](assets/add-person-to-blocklist-1.png)

1. 选择 **智能列表**.

   ![](assets/add-person-to-blocklist-2.png)

1. 命名您的列表，然后单击 **创建**.

   ![](assets/add-person-to-blocklist-3.png)

1. 将所有人员添加到您的 **智能列表** 您希望将添加到阻止列表。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >您阻止列表的人员不会收到操作电子邮件。

1. 返回您的项目。

   ![](assets/add-person-to-blocklist-5.png)

1. 单击 **新建** 并选择 **新建智能营销活动**.

   ![](assets/add-person-to-blocklist-6.png)

1. 为命名 **新建智能营销活动**. 单击&#x200B;**创建**。

   ![](assets/add-person-to-blocklist-7.png)

1. 拖放 **智能列表的成员**.

   ![](assets/add-person-to-blocklist-8.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/add-person-to-blocklist-9.png)

1. 单击 **流量** 选项卡。 拖放 **更改数据值** 流程操作。

   ![](assets/add-person-to-blocklist-10.png)

1. 在 **属性** 下拉选择 **已列出阻止** 并设置 **新值** 到 **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. 单击 **计划** 选项卡并选择 **运行一次**.

   ![](assets/add-person-to-blocklist-12.png)

1. 选择 **立即运行** 并单击 **运行**.

   ![](assets/add-person-to-blocklist-13.png)

1. 单击 **运行** 再来一次。

   ![](assets/add-person-to-blocklist-14.png)

这些用户将不再收到电子邮件。

>[!TIP]
>
>创建 [触发智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) 使用 **更改数据值** 替换为 **列入阻止为true** 面向所有未来具有阻止列表属性的人。
