---
unique-page-id: 1147066
description: 覆盖Smart Campaign中的人员限制 — Marketo文档 — 产品文档
title: 覆盖智能营销活动中的人员限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# 覆盖智能营销活动中的人员限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage允许您设置符合Smart Campaign资格的最大人数；这有助于避免意外地向整个数据库发送电子邮件。 如果要&#x200B;_覆盖_&#x200B;此限制，请按以下步骤操作。

>[!PREREQUISITES]
>
>请确保在Marketo管理员中[为智能营销活动启用人员限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"}。

1. 在&#x200B;**[!UICONTROL 营销活动]**&#x200B;中，转到您的Smart Campaign并单击&#x200B;**[!UICONTROL 计划]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. 在“Smart Campaign设置”中，单击&#x200B;**[!UICONTROL 编辑]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >默认限制为在Admin中设置的限制。

1. 输入新限制并单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   如果符合条件的人数超过设置的限制，则智能营销活动不会运行。

   >[!CAUTION]
   >
   >使用此功能时请务必小心，以免意外包含太多人。
