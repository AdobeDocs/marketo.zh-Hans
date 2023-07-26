---
unique-page-id: 2359793
description: 在社交促销活动中使用电子邮件 — Marketo文档 — 产品文档
title: 在社交促销活动中使用电子邮件
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 在社交促销活动中使用电子邮件 {#use-emails-in-social-promotions}

当您创建 [推荐优惠](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) 或 [抽奖](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以包含要在人员注册时发送的电子邮件，以及在人员赢得奖励时再次发送的电子邮件。

>[!TIP]
>
>要创建电子邮件，请参阅 [发送电子邮件爆料](/help/marketo/getting-started/quick-wins/send-an-email.md).

在电子邮件中，使用以下令牌：

* **注册电子邮件**：使用 **`{{social.Share Url}}`** 以向每位参与人员发送个性化共享链接。

* **履行电子邮件**：使用 **`{{social.Promo Code}}`** ，将每个入选者发送 [促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>在将电子邮件添加到社交应用程序之前，必须 _可操作_ 和 _已批准_. 请参阅 [编辑电子邮件的设置](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

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
   >当人员注册时，会自动发送确认电子邮件。

1. 添加履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. 在推荐优惠中，选择是自动还是手动发送履行电子邮件。

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>在抽奖活动中，履行电子邮件始终会在您完成任务时自动发送 [选择入选者](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**条件**
>
>* **自动完成目标**：当每个参与者满足目标时，将自动发送完成电子邮件。
>* **手动发送**：一旦人们开始实现目标，请手动返回您的反向链接选件 [发送履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>接下来，您可以 [选择共享URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) 或者，在推荐优惠中，您可以 [上传促销代码](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) 你会派人去的。
