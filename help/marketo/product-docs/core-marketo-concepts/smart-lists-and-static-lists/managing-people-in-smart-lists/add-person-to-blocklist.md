---
unique-page-id: 9438139
description: 将人员添加到阻止列表- Marketo文档 — 产品文档
title: 将人员添加到阻止列表
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 将人员添加到阻止列表 {#add-person-to-blocklist}

将人员添加到您的阻止列表会阻止他们接收您的信件。

1. 创建新的[默认程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"}并将其命名为“添加到阻止列表”。

1. 单击&#x200B;**[!UICONTROL 新建]**&#x200B;并选择&#x200B;**[!UICONTROL 新建本地资产]**。

   ![](assets/add-person-to-blocklist-1.png)

1. 选择&#x200B;**[!UICONTROL 智能列表]**。

   ![](assets/add-person-to-blocklist-2.png)

1. 命名您的列表，然后单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/add-person-to-blocklist-3.png)

1. 将所有要添加到阻止列表的人员添加到您的智能列表。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >您阻止列表的人员不会收到操作电子邮件。

1. 返回您的项目。

   ![](assets/add-person-to-blocklist-5.png)

1. 单击&#x200B;**[!UICONTROL 新建]**，然后选择&#x200B;**[!UICONTROL 新建Smart Campaign]**。

   ![](assets/add-person-to-blocklist-6.png)

1. 命名新的Smart Campaign。 单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/add-person-to-blocklist-7.png)

1. 拖放智能列表&#x200B;**的**&#x200B;成员。

   ![](assets/add-person-to-blocklist-8.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/add-person-to-blocklist-9.png)

1. 单击&#x200B;**[!UICONTROL 流量]**&#x200B;选项卡。 拖放&#x200B;**[!UICONTROL 更改数据值]**&#x200B;流程操作。

   ![](assets/add-person-to-blocklist-10.png)

1. 在&#x200B;**[!UICONTROL 属性]**&#x200B;下拉列表中，选择&#x200B;**[!UICONTROL 已列出]**&#x200B;块，并将&#x200B;**[!UICONTROL 新值]**&#x200B;设置为&#x200B;**[!UICONTROL true]**。

   ![](assets/add-person-to-blocklist-11.png)

1. 单击&#x200B;**[!UICONTROL 计划]**&#x200B;选项卡并选择&#x200B;**[!UICONTROL 运行一次]**。

   ![](assets/add-person-to-blocklist-12.png)

1. 选择&#x200B;**[!UICONTROL 立即运行]**，然后单击&#x200B;**[!UICONTROL 运行]**。

   ![](assets/add-person-to-blocklist-13.png)

1. 再次单击&#x200B;**[!UICONTROL 运行]**。

   ![](assets/add-person-to-blocklist-14.png)

这些用户将不再收到电子邮件。

>[!TIP]
>
>使用&#x200B;**更改数据值**&#x200B;创建一个[触发器营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}，其中列出的&#x200B;**块为true**，适用于将来具有可阻止列表属性的所有人员。
