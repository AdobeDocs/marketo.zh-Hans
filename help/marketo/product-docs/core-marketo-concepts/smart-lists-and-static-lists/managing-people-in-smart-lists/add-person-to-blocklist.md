---
unique-page-id: 9438139
description: 将人员添加到阻止列表- Marketo文档 — 产品文档
title: 将人员添加到阻止列表
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# 将人员添加到阻止列表 {#add-person-to-blocklist}

将人员添加到您的阻止列表会阻止他们接收您的信件。

1. 新建 [默认程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} 将其命名为“添加到阻止列表”。

1. 单击 **[!UICONTROL 新建]** 并选择 **[!UICONTROL 新建本地资产]**.

   ![](assets/add-person-to-blocklist-1.png)

1. 选择 **[!UICONTROL 智能列表]**.

   ![](assets/add-person-to-blocklist-2.png)

1. 命名您的列表，然后单击 **[!UICONTROL 创建]**.

   ![](assets/add-person-to-blocklist-3.png)

1. 将所有要添加到阻止列表的人员添加到您的智能列表。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >您阻止列表的人员不会收到操作电子邮件。

1. 返回您的项目。

   ![](assets/add-person-to-blocklist-5.png)

1. 单击 **[!UICONTROL 新建]** 并选择 **[!UICONTROL 新建智能营销活动]**.

   ![](assets/add-person-to-blocklist-6.png)

1. 命名新的Smart Campaign。 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/add-person-to-blocklist-7.png)

1. 拖放 **[!UICONTROL 智能列表的成员]**.

   ![](assets/add-person-to-blocklist-8.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/add-person-to-blocklist-9.png)

1. 单击 **[!UICONTROL 流量]** 选项卡。 拖放 **[!UICONTROL 更改数据值]** 流程操作。

   ![](assets/add-person-to-blocklist-10.png)

1. 在 **[!UICONTROL 属性]** 下拉选择 **[!UICONTROL 已列出阻止]** 并设置 **[!UICONTROL 新值]** 到 **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. 单击 **[!UICONTROL 计划]** 选项卡并选择 **[!UICONTROL 运行一次]**.

   ![](assets/add-person-to-blocklist-12.png)

1. 选择 **[!UICONTROL 立即运行]** 并单击 **[!UICONTROL 运行]**.

   ![](assets/add-person-to-blocklist-13.png)

1. 单击 **[!UICONTROL 运行]** 再来一次。

   ![](assets/add-person-to-blocklist-14.png)

这些用户将不再收到电子邮件。

>[!TIP]
>
>创建 [触发营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} 使用 **更改数据值** 替换为 **列入阻止为true** 面向所有未来具有阻止列表属性的人。
