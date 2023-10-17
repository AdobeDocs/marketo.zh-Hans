---
unique-page-id: 1146978
description: 在等待流步骤中使用持续时间 — Marketo文档 — 产品文档
title: 在等待流步骤中使用持续时间
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 1%

---

# 在等待流步骤中使用持续时间 {#use-a-duration-in-a-wait-flow-step}

您可以使用等待流步骤暂停人员通过智能营销活动进行一段特定时间的旅程。 您还可以指定星期几和结束时间的标准。

1. 在您的Smart Campaign中 **[!UICONTROL 流量]** 选项卡，拖动到 **[!UICONTROL 等待]** 流程步骤。

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. 输入要暂停的时间。

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. 就是这样！ 流将暂停指定的持续时间。 对于高级选项，单击右侧的齿轮图标。

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. 指定在一周中等待步骤应该结束的日期。

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. （可选）指定时间。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**示例**
   >
   >周五，下午5点，系统会触发一个Smart Campaign。 等待步骤是高级步骤：48小时，必须在周一至周五上午9点结束。
   >
   >结果是，该人员将继续流入流道。 **周一上午9点**. 这是48小时后的第一个M-F日期。

   >[!NOTE]
   >
   >使用的持续时间、日期、时间和天数均基于您的订阅所在时区。

   >[!MORELIKETHIS]
   >
   >* [在等待流步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
