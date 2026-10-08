---
unique-page-id: 2360243
description: 设置符合Smart Campaign资格的最大人数，以避免意外地通过电子邮件发送整个数据库。
title: 为智能营销活动启用人员限制
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/6VwkOwN9nTqSyNcXvzyggPTk0Um5x1GPXIp2DBf2kww'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
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
   >此限制适用于所有智能营销活动，但可以在营销活动级别覆盖。 了解如何在Smart Campaign[&#128279;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)中覆盖人员限制。

>[!MORELIKETHIS]
>
>[在智能营销活动中覆盖人员限制](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
