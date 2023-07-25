---
unique-page-id: 1146978
description: 在等待流步骤中使用持续时间 — Marketo文档 — 产品文档
title: 在等待流步骤中使用持续时间
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 在等待流步骤中使用持续时间 {#use-a-duration-in-a-wait-flow-step}

您可以使用等待流量步骤在特定时间内暂停人员通过智能营销活动的历程。 您还可以指定星期几和结束时间的标准。

1. 在您的智能营销活动中 **流量** 选项卡，拖动到 **等待** 流程步骤。

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. 输入要暂停的时间。

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. 就是这样！ 流将暂停指定的持续时间。 对于高级选项，单击右侧的齿轮图标。

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. 指定在一周中等待步骤应该结束的日期。

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. （可选）指定时间。 单击 **保存**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**示例**
   >
   >有人在周五下午5点触发一场明智的营销活动。 等待步骤是高级步骤：48小时，必须在周一至周五上午9点结束。
   >
   >结果是，该人员将继续流入该流 **星期一，上午9点**. 这是48小时后的第一个M-F日期。

   >[!NOTE]
   >
   >使用的持续时间、日期、时间和天数均基于您的订阅所在时区。

   >[!MORELIKETHIS]
   >
   >* [在等待流步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
