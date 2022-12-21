---
unique-page-id: 1147066
description: 在智能促销活动中覆盖人员限制 — Marketo文档 — 产品文档
title: 在智能营销活动中覆盖人员限制
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# 在智能营销活动中覆盖人员限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo允许您设置符合智能营销活动资格的最大人员数；这有助于您避免意外地向整个数据库发送电子邮件。 如果您想 _覆盖_ 这个限制，这就是方法。

>[!PREREQUISITES]
>
>一定要 [启用智能促销活动的人员限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) 在Marketo管理员中。

1. 在营销活动中，转到您的智能营销活动，然后单击 **计划**.

   ![](assets/one.png)

1. 在智能营销活动设置中，单击 **编辑**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >默认限制为在“管理员”中设置的限制。

1. 输入新限制，然后单击 **保存。**

   ![](assets/three.png)

   如果符合条件的人数超过设置的限制，则不会运行智能营销活动。

   >[!CAUTION]
   >
   >使用此功能时要小心，这样您就不会意外包含太多人员。
