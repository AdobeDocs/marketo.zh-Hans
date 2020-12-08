---
unique-page-id: 2359791
description: 指定推荐优惠的目标- Marketo Docs —— 产品文档
title: 指定引用优惠的目标
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# 指定引用优惠的目标 {#specify-goal-for-referral-offer}

创建 [推荐优惠时](create-a-referral-offer.md)，您需要定义履行目标。 目标可以由网页上的人员活动（如页面访问或注册）来定义。 您甚至可以使用自 [定义JavaScript事件](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)。

或者，您也可以在Market [中使用智能列表触发器](specify-goal-for-referral-offer.md) ，以等待任何里程碑，如为引用人员创建的机会。

目标示例：

* 10次推荐访问
* 5个引用的注册
* 已创建1个转发机会
* 2个引用的电子商务购买
* 5位参加网络研讨会的与会者

1. 转到营 **销活动**。

   ![](assets/ma.png)

1. 选择参照优惠，然后单击“编 **辑草稿”。**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在引用优惠编辑器中，转到“应用程 **序设置** ”>“ **优惠详细信息”。**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 在“ **设置**”下，从“实施目 **标** ”下拉菜单中选择一个事件类型。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您计划使用“将信 **用授予推荐人流** ”步骤，则必须选择“智 **能列表触发器** ”作为此处的实施目标类型。

* 引荐访问：优惠参加者每次从朋友访问托管优惠的页面时都会获得积分。
* 引用的注册：优惠参加者可以为注册优惠的每个朋友获得积分。
* 智能列表触发器：优惠参加者可以为在智能活动中满足智能 [列表触发](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) 条件的每 [个朋友获奖](http://docs.marketo.com/display/docs/smart+campaigns)。 例如，您可以使用触发器，当引用的潜在客户注册参加网络研讨会时触发。

* 自定义JavaScript事件:优惠参加者可以因在您的页面上触发定义的JavaScript事件的每个朋友而获得积分。 请参 [阅自定义事件的转换脚本](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>智能活动中提供了新的过滤器和触发器，可用于监控社交活动。 请参 [阅将触发器和过滤器用于社交活动](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>**相关文章**
>
>接下来，您可 [以选择要从您的推荐优惠发送的注册](send-referral-offer-fulfillment-email.md) 和实施电子邮件。

