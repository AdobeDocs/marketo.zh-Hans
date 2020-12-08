---
unique-page-id: 7513680
description: 自动发出针对可能的重复的警报- Marketo Docs —— 产品文档
title: 自动提醒可能的重复
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# 自动提醒可能的重复 {#automate-an-alert-for-possible-duplicate-people}

每次可能创建重复人时都需要提醒？ 下面介绍如何设置智能活动。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

1. [创建新的智能活动](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)。 定义以下智能列表:

   * 触发器： **已创建人员**
   * 过滤器：**重复字段。 **字段名 **称****为全名**。

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >发挥创意。 用不同的场进行实验，获得更好的滤波效果。

1. 在流步骤中，选择“发送 [警报流](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) ”操作。

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >使用“ [发送警报信息](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) ”令牌在CRM中包含指向该人员的链接。

   >[!CAUTION]
   >
   >如果导入大列表，您可能会同时收到大量这些警报！
   >
   >
   >另外，两个同名的人并不自动表示他们是同一个人。

1. 在“活动”选项卡 **中激活** “计划”。

   ![](assets/image2017-3-27-8-3a24-3a37.png)

就这样！ 每次在Marketo中创建具有现有全名的新人时，此智能活动都将触发。

>[!MORELIKETHIS]
>
>* [查找并合并重复](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

