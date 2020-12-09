---
unique-page-id: 2359793
description: 在社交促销- Marketo Docs —— 产品文档中使用电子邮件
title: 在社交促销中使用电子邮件
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---


# 在社交促销中使用电子邮件 {#use-emails-in-social-promotions}

创建推荐 [优惠](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) 或抽奖 [时](../../../../product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以包含在用户注册时发送的电子邮件，以及在用户获得奖励后再发送。

>[!TIP]
>
>要创建电子邮件，请参 [阅发送电子邮件爆炸](../../../../getting-started/quick-wins/send-an-email.md)。

在电子邮件中，使用以下令牌：

* **注册电子邮件**:使用 **`{{social.Share Url}}`** 向每位参与者发送个性化的共享链接。

* **履行电子邮件**:使 **`{{social.Promo Code}}`** 用向每个入选方发送 [促销代码](use-promo-codes-for-offer-fulfillment.md)。

>[!PREREQUISITES]
>
>在向社交应用程序添加电子邮件之前，电子邮件必须 *可操作* 并 *获得批准*。 请参 [阅编辑电子邮件的设置](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

1. 转到营 **销活动**。

   ![](assets/ma.png)

1. 选择应用程序，然后单击“ **编辑草稿”**。

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交应用程序编辑器中，转到“应 **用程序设置”>“优惠详细信息** ”(或 **“抽奖详细信息**”)。

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
>在抽奖中，当您选择入选方时，将始终自动发 [送履行电子邮件](../../../../product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md)。

>[!NOTE]
>
>**定义**
>
>* **自动开启目标**:当每个参加者达到目标时，系统会自动发送履行电子邮件。
>* **手动发送**:当开始达到目标后，返回您的推荐优惠，手动发送 [履行电子邮件](../../../../product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)。

>



>[!NOTE]
>
>**相关文章**
>
>接下来，您可 [以选择共享URL](choose-the-share-url-for-a-social-app.md) ，或者在推荐优惠中，您 [可以上传要发送的](use-promo-codes-for-offer-fulfillment.md) 促销代码。

