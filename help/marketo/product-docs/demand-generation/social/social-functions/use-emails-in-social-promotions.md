---
unique-page-id: 2359793
description: 在社交促销活动中使用电子邮件 — Marketo文档 — 产品文档
title: 在社交促销活动中使用电子邮件
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 在社交促销活动中使用电子邮件 {#use-emails-in-social-promotions}

创建 [推荐选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) 或 [抽奖](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以在人员注册时发送电子邮件，也可以在人员获得奖励时再次发送电子邮件。

>[!TIP]
>
>要创建电子邮件，请参阅 [发送电子邮件爆炸](/help/marketo/getting-started/quick-wins/send-an-email.md).

在电子邮件中，使用以下令牌：

* **注册电子邮件**:使用 **`{{social.Share Url}}`** 向每个参与者发送个性化共享链接。

* **履行电子邮件**:使用 **`{{social.Promo Code}}`** 向每个入选者发送 [促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>在向社交应用程序添加电子邮件之前，必须 _操作_ 和 _已批准_. 请参阅 [编辑电子邮件的设置](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. 转到 **营销活动**.

   ![](assets/ma.png)

1. 选择应用程序，然后单击 **编辑草稿**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. 在社交应用程序编辑器中，转到 **应用程序设置>选件详细信息** (或 **抽奖详细信息**)。

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. 添加注册电子邮件。

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >当某人注册时，系统会自动发送确认电子邮件。

1. 添加履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 在推荐选件中，选择自动还是手动发送履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>在抽奖活动中，履行电子邮件始终在您 [选择入选者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**条件**
>
>* **自动实现目标**:当每位参与者均达到目标时，系统会自动发送履行电子邮件。
>* **手动发送**:人员开始达到目标后，请返回您的推荐选件以手动 [发送履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>


>[!MORELIKETHIS]
>
>接下来，您可以 [选择共享URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) 或者，在您的推荐选件中，您可以 [上传促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) 你会发出去的。
