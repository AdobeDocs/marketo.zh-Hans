---
unique-page-id: 1147066
description: 覆盖Smart Campaign中的人员限制 — Marketo文档 — 产品文档
title: 覆盖智能营销活动中的人员限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# 覆盖智能营销活动中的人员限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo允许您设置符合智能营销活动资格的最大人数；这有助于避免意外地通过电子邮件发送整个数据库。 如果您想要 _覆盖_ 这个限制，就是这样。

>[!PREREQUISITES]
>
>请确保 [为智能营销活动启用人员限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) 在Marketo Admin中。

1. 在营销活动中，转到您的智能营销活动并单击 **计划**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. 在Smart Campaign设置中，单击 **编辑**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >默认限制为在“管理员”中设置的限制。

1. 输入新限制，然后单击 **保存。**

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   如果符合条件的人数超过设置的限制，则智能营销活动将不会运行。

   >[!CAUTION]
   >
   >使用此功能时请务必小心，以免意外包含太多人。
