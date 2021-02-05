---
unique-page-id: 2359793
description: 在社交促销- Marketo Docs —— 产品文档中使用电子邮件
title: 在社交促销中使用电子邮件
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# 在社交促销中使用电子邮件{#use-emails-in-social-promotions}

当您创建[推荐优惠](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)或[抽奖](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)时，您可以包含在用户注册时发送的电子邮件，以及在用户获得奖励后再次发送电子邮件。

>[!TIP]
>
>要创建电子邮件，请参阅[发送电子邮件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md)。

在电子邮件中，使用以下令牌：

* **注册电子邮件**:使用 **`{{social.Share Url}}`** 向每位参与者发送个性化的共享链接。

* **履行电子邮件**:用 **`{{social.Promo Code}}`** 于向每个入选方发送 [促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)。

>[!PREREQUISITES]
>
>在向社交应用程序添加电子邮件之前，电子邮件必须是&#x200B;_operational_&#x200B;和&#x200B;_approved_。 请参阅[编辑电子邮件的设置](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

1. 转到&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 选择应用程序，然后单击“编辑草稿&#x200B;**”。**

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交应用程序编辑器中，转至&#x200B;**应用程序设置>优惠详细信息**（或&#x200B;**抽奖详细信息**）。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 添加注册电子邮件。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >当人员注册时，系统会自动发送确认电子邮件。

1. 添加履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 在推荐优惠中，选择自动还是手动发送履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>在抽奖中，当您[选择获胜者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)时，将始终自动发送履行电子邮件。

>[!NOTE]
>
>**定义**
>
>* **自动开启目标**:当每个参加者达到目标时，系统会自动发送履行电子邮件。
>* **手动发送**:当开始达到目标后，返回您的推荐优惠，手动发送 [履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)。

>



>[!MORELIKETHIS]
>
>接下来，您可以[选择共享URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)，或者在您的推荐优惠中，您可以[上传您将发出的促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md)。
