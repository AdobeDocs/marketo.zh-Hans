---
unique-page-id: 2359791
description: 指定引荐选件的目标 — Marketo文档 — 产品文档
title: 指定引荐选件的目标
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 指定引荐选件的目标 {#specify-goal-for-referral-offer}

当您 [创建反向链接选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)，则需要定义实现目标。 目标可由网页上的人员活动（如页面访问或注册）来定义。 您甚至可以使用 [自定义JavaScript事件](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

或者，您也可以使用Marketo中的智能列表触发器来等待任何里程碑，例如为引荐人员创建的机会。

示例目标：

* 10次推荐访问
* 5次引荐注册
* 已创建引荐机会
* 2次引荐电子商务购买
* 5名引荐的网络研讨会与会者

1. 转到 **营销活动**.

   ![](assets/ma.png)

1. 选择引荐选件，然后单击 **编辑草稿**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在推荐选件编辑器中，转到 **应用程序设置** > **选件详细信息**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 在 **设置**，从中选择事件类型 **实现目标** 下拉菜单。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您计划使用 **将点数给予反向链接** “流”步骤，您必须选择 **智能列表触发器** 作为此处的实现目标类型。

* 引荐访问：选件参与者每次从朋友访问托管您选件的页面时都会获得点数。
* 引荐注册：选件参与者将获得注册该选件的每个朋友的点数。
* 智能列表触发器：选件参与者将获得符合 [智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) 触发器 [智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). 例如，您可以使用一个触发器，该触发器将在推荐的潜在客户注册参加网络研讨会时触发。

* 自定义JavaScript事件：选件参与者将获得在您的页面上触发定义JavaScript事件的每个朋友的点数。 请参阅 [自定义事件的转换脚本](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>智能营销活动中提供了新的过滤器和触发器，可用于监控社交活动。 请参阅 [对社交活动使用触发器和过滤器](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>接下来，您可以 [选择注册和履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) 以从您的推荐选件发送。
