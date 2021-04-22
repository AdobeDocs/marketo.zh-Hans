---
unique-page-id: 1146978
description: 在等待流程步骤中使用持续时间 — Marketo Docs — 产品文档
title: 在等待流步骤中使用持续时间
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 在等待流步骤{#use-a-duration-in-a-wait-flow-step}中使用持续时间

您可以使用等待流程步骤在特定时间段内暂停个人通过智能活动的旅程。 您还可以指定一周中的某天和结束时的条件。

1. 在您的智能活动&#x200B;**流**&#x200B;选项卡中，拖动到&#x200B;**等待**&#x200B;流步骤上。

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. 输入要暂停的时间。

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. 就这样！ 流将在您指定的持续时间内暂停。 对于高级选项，单击右侧的齿轮图标。

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. 指定等待步骤应结束的一周中的某天。

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. （可选）指定时间。 单击&#x200B;**保存**。

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**示例**
   >
   >周五下午5点，有人触发了智能活动。 等待步骤是高级的：48小时，必须在周一至周五早9点结束。
   >
   >结果是，该人将在&#x200B;**星期一上午9点**&#x200B;继续流动。 这是48小时后的第一次M-F约会。

   >[!NOTE]
   >
   >使用的持续时间、日期、时间和天数均基于订阅的时区。

   >[!MORELIKETHIS]
   >
   >* [在等待流程步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [在等待流步骤中使用日期令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)

