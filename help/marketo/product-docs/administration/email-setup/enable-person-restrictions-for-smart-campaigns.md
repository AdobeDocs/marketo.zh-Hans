---
unique-page-id: 2360243
description: 设置符合Smart Campaign资格的最大人数，以避免意外地通过电子邮件发送整个数据库。
title: 为智能营销活动启用人员限制
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
source-git-commit: df76402e5fb0c002afeb04d41c52801be67a7136
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 14%

---

# 为智能营销活动启用人员限制 {#enable-person-restrictions-for-smart-campaigns}

Marketo中有一个功能，用于限制符合Smart Campaign资格的最多&#x200B;_个_&#x200B;人数。 这样可避免意外地向整个数据库发送电子邮件。

>[!NOTE]
>
>**需要管理员权限**

>[!CAUTION]
>
>这仅适用于批量营销活动和电子邮件项目。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/enable-person-restrictions-for-smart-campaigns-1.png)

1. 单击 **[!UICONTROL Smart Campaign]**。

   ![](assets/enable-person-restrictions-for-smart-campaigns-2.png)

1. 单击 **[!UICONTROL Edit]**。

   ![](assets/enable-person-restrictions-for-smart-campaigns-3.png)

   >[!CAUTION]
   >
   >如果符合条件通过Smart Campaign运行的人数超过设置的限制，则它根本不会运行。

1. 输入限制并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/enable-person-restrictions-for-smart-campaigns-4.png)

   >[!TIP]
   >
   >将此字段留空可禁用此功能。

   >[!CAUTION]
   >
   >此限制适用于所有智能营销活动，但可以在营销活动级别覆盖。 了解如何在Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)中[覆盖人员限制。

>[!MORELIKETHIS]
>
>[在智能营销活动中覆盖人员限制](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
