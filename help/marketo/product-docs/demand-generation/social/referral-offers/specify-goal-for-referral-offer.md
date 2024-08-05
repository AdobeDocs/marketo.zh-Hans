---
unique-page-id: 2359791
description: 指定推荐服务的目标 — Marketo文档 — 产品文档
title: 指定推荐服务的目标
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 指定推荐服务的目标 {#specify-goal-for-referral-offer}

当您[创建反向链接选件](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)时，需要定义完成目标。 目标可以通过网页上的人员活动（如页面访问或注册）来定义。 您甚至可以使用[自定义JavaScript事件](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)。

>[!IMPORTANT]
>
>2024年7月31日，我们启动了停用此功能的过程。 您将无法创建新资源。 现有资产将继续运作至2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

或者，您可以在Marketo Engage中使用智能列表触发器等待任何里程碑，例如为被引用人员创建的业务机会。

目标示例：

* 10次转介访问
* 5个推荐注册
* 已创建1个被推荐商机
* 2个推荐的电子商务购买
* 5位推荐的网络研讨会与会者

1. 转到&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 选择推荐优惠，然后单击&#x200B;**编辑草稿**。

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 在推荐优惠编辑器中，转到&#x200B;**应用程序设置** > **优惠详细信息**。

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 在&#x200B;**设置**&#x200B;下，从&#x200B;**实现目标**&#x200B;下拉列表中选择一个事件类型。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>如果您计划使用&#x200B;**向推荐人提供信用**&#x200B;流程步骤，则必须在此处选择&#x200B;**智能列表触发器**&#x200B;作为履行目标类型。

* 转荐访问：每当好友访问托管您的优惠的页面时，优惠参与者就会获得积分。
* 引荐注册：优惠参与者会为注册优惠的每个朋友获得积分。
* 智能列表触发器：对于在[智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)中满足[智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)触发条件的每个朋友，优惠参与者均可获取积分。 例如，您可以使用被引用的目标客户注册网络研讨会时触发的触发器。

* 自定义JavaScript事件：为参与人提供积分给在页面上触发已定义JavaScript事件的每个好友。 查看自定义事件的[转换脚本](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>智能营销活动中提供了新的筛选器和触发器以监控社交活动。 请参阅[为社交活动使用触发器和过滤器](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!MORELIKETHIS]
>
>接下来，您可以[从您的推荐优惠中选择要发送的注册和履行电子邮件](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)。
