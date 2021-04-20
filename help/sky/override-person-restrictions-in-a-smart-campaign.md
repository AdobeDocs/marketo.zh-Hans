---
title: override-person-restrictions-in-a-smart-活动
description: 在智能活动中覆盖人员限制
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---

# 在智能活动中覆盖人员限制

<br> 

Marketo允许您设置最多可以获得智能活动的人数；这有助于您避免意外通过电子邮件发送整个数据库。 如果要覆盖此限制，请按照以下方式操作。

>[!IMPORTANT]
>
>请务必[为Marketo [!UICONTROL Admin]中的智能活动](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns)启用人员限制。

1. 找到您的智能活动并单击&#x200B;**[!UICONTROL Schedule]**。

   ![图像1](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. 单击&#x200B;**[!UICONTROL Qualification Rules]**。

   ![图2](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >默认限制是在“管理”中设置的限制。

1. 在&#x200B;**[!UICONTROL Abort campaign if qualified leads exceed]**&#x200B;旁，输入新限制。

   ![图3](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>如果符合条件的人员数量超过设置的限制，智能活动将不运行。

>[!CAUTION]
>
>使用此功能时要小心，以免意外包含过多人。
