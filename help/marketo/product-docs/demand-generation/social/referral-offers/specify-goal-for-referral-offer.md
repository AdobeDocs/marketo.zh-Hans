---
unique-page-id: 2359791
description: 指定反向链接选件的目标 — Marketo文档 — 产品文档
title: 指定反向链接选件的目标
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 指定反向链接选件的目标 {#specify-goal-for-referral-offer}

当您 [创建反向链接选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)，您需要定义实现目标。 目标可由网页上的人员活动定义，如页面访问或注册。 您甚至可以使用 [自定义JavaScript事件](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

或者，您可以使用Marketo中的智能列表触发器来等待任何里程碑，例如为被引荐人员创建的商机。

目标示例：

* 10次转介访问
* 5个引用的注册
* 已创建1个引用的机会
* 2次引用的电子商务购买
* 5位推荐的网络研讨会与会者

1. 转到 **营销活动**.

   ![](assets/ma.png)

1. 选择反向链接选件，然后单击 **编辑草稿**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在反向链接选件编辑器中，转到 **应用程序设置** > **优惠详细信息**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 下 **设置**，从中选择一个事件类型 **实现目标** 下拉菜单。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您计划使用 **将点数提供给反向链接** 流步骤，您必须选择 **智能列表触发器** 作为实现目标类型。

* 反向访问：对于朋友访问您的选件所在的页面，每次访问都向选件参与者提供点数。
* 引用的注册：优惠参与者可以获得每个注册优惠的朋友的点数。
* 智能列表触发器：为符合条件的每个朋友提供点数 [智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) 中的触发器 [智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). 例如，您可以使用触发器，该触发器在被引用的潜在客户注册参加网络研讨会时触发。

* 自定义JavaScript事件：对于在页面上触发定义的JavaScript事件的每个朋友，优惠参与者可获得点数。 请参阅 [自定义事件的转换脚本](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>智能营销活动中提供了新的筛选器和触发器以监控社交活动。 请参阅 [对社交活动使用触发器和过滤器](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>接下来，您可以 [选择注册和履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) 以发送您的推荐选件。
