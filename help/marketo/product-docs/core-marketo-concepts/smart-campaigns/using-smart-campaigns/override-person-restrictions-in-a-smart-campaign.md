---
unique-page-id: 1147066
description: 了解如何在Smart Campaign中覆盖人员限制。 允许人员即使达到通信限制也能运行。
title: 在智能营销活动中覆盖人员限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 141
ht-degree: 9%

---

# 在智能营销活动中覆盖人员限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage允许您设置符合Smart Campaign资格的最大人员数；这有助于避免意外地向整个数据库发送电子邮件。 如果要&#x200B;_覆盖_&#x200B;此限制，请按以下步骤操作。

>[!PREREQUISITES]
>
>请确保在Marketo管理员中[为智能营销活动启用人员限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"}。

1. 在&#x200B;**[!UICONTROL Marketing Activities]**&#x200B;中，转到您的Smart Campaign并单击&#x200B;**[!UICONTROL Schedule]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. 在Smart Campaign设置中，单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >默认限制为在Admin中设置的限制。

1. 输入新限制并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   如果符合条件的人数超过设置的限制，则智能营销活动不会运行。

   >[!CAUTION]
   >
   >使用此功能时请务必小心，以免意外包含太多人。
