---
unique-page-id: 9438139
description: 将人员添加到阻止列表- Marketo文档 — 产品文档
title: 将人员添加到阻止列表
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 10%

---

# 将人员添加到阻止列表 {#add-person-to-blocklist}

将人员添加到您的阻止列表会阻止他们接收您的信件。

1. 创建新的[默认程序](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"}并将其命名为“添加到阻止列表”。

1. 单击&#x200B;**[!UICONTROL New]**&#x200B;并选择&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/add-person-to-blocklist-1.png)

1. 选择 **[!UICONTROL Smart List]**。

   ![](assets/add-person-to-blocklist-2.png)

1. 命名列表并单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/add-person-to-blocklist-3.png)

1. 将所有要添加到阻止列表的人员添加到您的智能列表。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >您阻止列表的人员不会收到操作电子邮件。

1. 返回您的项目。

   ![](assets/add-person-to-blocklist-5.png)

1. 单击&#x200B;**[!UICONTROL New]**&#x200B;并选择&#x200B;**[!UICONTROL New Smart Campaign]**。

   ![](assets/add-person-to-blocklist-6.png)

1. 命名新的Smart Campaign。 单击 **[!UICONTROL Create]**。

   ![](assets/add-person-to-blocklist-7.png)

1. 拖放&#x200B;**[!UICONTROL Member of Smart List]**。

   ![](assets/add-person-to-blocklist-8.png)

1. 选择您刚刚创建的智能列表。

   ![](assets/add-person-to-blocklist-9.png)

1. 单击 **[!UICONTROL Flow]** 选项卡。拖放&#x200B;**[!UICONTROL Change Data Value]**&#x200B;流量操作。

   ![](assets/add-person-to-blocklist-10.png)

1. 在&#x200B;**[!UICONTROL Attribute]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Block Listed]**&#x200B;并将&#x200B;**[!UICONTROL New Value]**&#x200B;设置为&#x200B;**[!UICONTROL true]**。

   ![](assets/add-person-to-blocklist-11.png)

1. 单击&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡并选择&#x200B;**[!UICONTROL Run Once]**。

   ![](assets/add-person-to-blocklist-12.png)

1. 选择 **[!UICONTROL Run Now]** 并点击 **[!UICONTROL Run]**。

   ![](assets/add-person-to-blocklist-13.png)

1. 再次单击&#x200B;**[!UICONTROL Run]**。

   ![](assets/add-person-to-blocklist-14.png)

这些用户将不再收到电子邮件。

>[!TIP]
>
>使用[更改数据值](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}创建一个&#x200B;**触发器营销活动**，其中列出的&#x200B;**块为true**，适用于将来具有可阻止列表属性的所有人员。
