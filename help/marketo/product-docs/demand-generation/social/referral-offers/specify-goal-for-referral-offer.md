---
unique-page-id: 2359791
description: 指定推荐优惠的目标- Marketo Docs —— 产品文档
title: 指定引用优惠的目标
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# 指定引用优惠的目标{#specify-goal-for-referral-offer}

当[创建引用优惠](create-a-referral-offer.md)时，您需要定义实现目标。 目标可以由网页上的人员活动（如页面访问或注册）来定义。 您甚至可以使用[自定义JavaScript事件](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)。

或者，您也可以在Market中使用[智能列表触发器](specify-goal-for-referral-offer.md)等待任何里程碑，如为引用的人创建的机会。

目标示例：

* 10次推荐访问
* 5个引用的注册
* 已创建1个转发机会
* 2个引用的电子商务购买
* 5位参加网络研讨会的与会者

1. 转到&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 选择引用优惠，然后单击“编辑草稿”。****

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在引用优惠编辑器中，转至&#x200B;**应用程序设置** > **优惠详细信息。**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 在&#x200B;**设置**&#x200B;下，从&#x200B;**实施目标**&#x200B;下拉菜单中选择事件类型。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您计划使用&#x200B;**将信用授予推荐人**&#x200B;流步骤，则必须选择&#x200B;**智能列表触发器**&#x200B;作为此处的实现目标类型。

* 引荐访问：优惠参加者每次从朋友访问托管优惠的页面时都会获得积分。
* 引用的注册：优惠参加者可以为注册优惠的每个朋友获得积分。
* 智能列表触发器：优惠参加者可以为满足[智能列表](http://docs.marketo.com/display/docs/smart+campaigns)中[智能活动](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)触发条件的每个朋友获得积分。 例如，您可以使用触发器，当引用的潜在客户注册参加网络研讨会时触发。

* 自定义JavaScript事件:优惠参加者可以因在您的页面上触发定义的JavaScript事件的每个朋友而获得积分。 请参阅自定义事件的[转换脚本](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>智能活动中提供了新的过滤器和触发器，可用于监控社交活动。 请参阅[使用社交活动的触发器和过滤器](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!MORELIKETHIS]
>
>接下来，您可以[选择要从您的推荐优惠发送的注册和实施电子邮件](send-referral-offer-fulfillment-email.md)。

