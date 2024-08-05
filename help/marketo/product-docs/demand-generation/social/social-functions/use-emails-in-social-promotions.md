---
unique-page-id: 2359793
description: 在社交促销活动中使用电子邮件 — Marketo文档 — 产品文档
title: 在社交促销活动中使用电子邮件
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 在社交促销活动中使用电子邮件 {#use-emails-in-social-promotions}

当您创建[推荐选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)或[抽奖](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)时，您可以包含要在人员注册时发送的电子邮件，以及在人员赢得奖励时再次发送的电子邮件。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 无法再创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!TIP]
>
>若要创建电子邮件，请参阅[发送电子邮件爆炸邮件](/help/marketo/getting-started/quick-wins/send-an-email.md)。

在电子邮件中，使用以下令牌：

* **注册电子邮件**：使用&#x200B;**`{{social.Share Url}}`**&#x200B;向每位参与人员发送个性化共享链接。

* **履行电子邮件**：使用&#x200B;**`{{social.Promo Code}}`**&#x200B;向每位入选者发送[促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)。

>[!PREREQUISITES]
>
>在将电子邮件添加到社交应用之前，该电子邮件必须是&#x200B;_可操作的_&#x200B;和&#x200B;_已批准的_。 请参阅[编辑电子邮件的设置](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

1. 转到&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 选择应用程序，然后单击&#x200B;**编辑草稿**。

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交应用程序编辑器中，转到&#x200B;**应用程序设置>优惠详细信息**（或&#x200B;**抽奖详细信息**）。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 添加注册电子邮件。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >当人员注册时，会自动发送确认电子邮件。

1. 添加履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 在推荐优惠中，选择是自动还是手动发送履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>在抽奖活动中，当您[选择入选者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)时，始终会自动发送履行电子邮件。

>[!NOTE]
>
>**定义**
>
>* 目标&#x200B;**上的**&#x200B;自动：当每位参与者都达到目标时，将自动发送完成电子邮件。
>* **手动发送**：一旦人们开始实现目标，请返回您的反向链接选件以手动[发送履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)。
>

>[!MORELIKETHIS]
>
>接下来，您可以[选择共享URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)，或者在您的推荐选件中，您可以[上传将要发送的促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)。
