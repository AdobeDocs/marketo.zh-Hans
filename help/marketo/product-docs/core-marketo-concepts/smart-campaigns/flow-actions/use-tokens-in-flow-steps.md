---
unique-page-id: 1146995
description: 在流程步骤中使用令牌 — Marketo文档 — 产品文档
title: 在流程步骤中使用令牌
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# 在流程步骤中使用令牌 {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[向智能营销活动添加流量步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

令牌是一个变量。 您可以将其用于电子邮件、登陆页面和智能营销策划中，以便简化您的工作。 您可以使用 [我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) （自定义令牌）定义在流程步骤、Webhook、电子邮件和登陆页面中。 您可以使用令牌在以下流程步骤中包含变量内容：

* 更改数据值
* 更改项目群成员数据
* 有趣的时刻
* Salesforce Campaign步骤（添加、删除、更改状态）
* 创建任务
* 发送警报（仅在触发营销活动中）

1. 在流程步骤中，开始键入 `{{` 以获取令牌类别。

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >签出 [令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) 以获取多个可用令牌的列表。

1. 继续键入，直到找到所需的令牌并单击进行选择。

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >多个令牌可用于“有趣的时刻”、“创建任务”和“发送警报”流程步骤。

   >[!NOTE]
   >
   >项目群成员自定义字段令牌可用于：创建任务、在Microsoft中创建任务、有趣的时刻、更改数据值流程操作和Webhook。

   酷！ 运行智能营销活动时，将从令牌中提取数据。

   >[!MORELIKETHIS]
   >
   >* [管理我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [了解项目中的我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)
