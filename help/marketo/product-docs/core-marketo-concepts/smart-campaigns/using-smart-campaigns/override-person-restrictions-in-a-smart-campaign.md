---
unique-page-id: 1147066
description: 在智能活动中覆盖人员限制- Marketo Docs —— 产品文档
title: 在智能活动中覆盖人员限制
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# 在智能活动中覆盖人员限制 {#override-person-restrictions-in-a-smart-campaign}

Marketo允许您设置最大* *可以获得智能活动的人数；这有助于您避免意外发送整个数据库的电子邮件。 如果要覆 *盖* 此限制，请按如下方式。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**先决条件**
>
>请务必在Marketo [Admin中为智能活动启](../../../../product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) 用人员限制。

1. 在营销活动中，转到** **智能活动并单击 **计划**。

   ![](assets/one.png)

   在智能活动设置中，单击编辑。
   ![](assets/two.png)

   >[!NOTE]
   >
   >默认限制是管理员中设置的限制。

1. 输入新限制，然后单击“保 **存”。**

   ![](assets/three.png)

   如果符合条件的人员数量超过设置的限制，智能活动将不运行。

   >[!CAUTION]
   >
   >使用此功能时要小心，这样您就不会意外包含太多人。

