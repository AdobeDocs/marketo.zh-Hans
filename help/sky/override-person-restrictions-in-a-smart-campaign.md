---
title: override-person-restrictions-in-a-smart-活动
description: 在智能活动中覆盖人员限制
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# 在智能活动中覆盖人员限制

<br> 

Marketo允许您设置可以获得智能活动的最大人数；这有助于您避免意外发送整个数据库的电子邮件。 如果要覆盖此限制，请按以下方式操作。

>[!IMPORTANT]
>
>请务必在Marketo [中为智能活动启用](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) “人员限制 [!UICONTROL Admin]”。

1. 查找您的智能活动并单击 [!UICONTROL **计划**]。

   ![图像1](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. 单击“ [!UICONTROL **资格规则**]”。

   ![图像2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >默认限制是管理员中设置的限制。

1. 如果合格 [!UICONTROL **潜在客户超过，则在中止活动**]，输入新限制。

   ![图3](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>如果符合条件的人员数量超过设置的限制，智能活动将不运行。

>[!CAUTION]
>
>使用此功能时要小心，这样您就不会意外包含太多人。
