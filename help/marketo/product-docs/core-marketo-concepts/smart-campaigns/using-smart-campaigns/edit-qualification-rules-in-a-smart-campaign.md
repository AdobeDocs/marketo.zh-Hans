---
unique-page-id: 1146974
description: 在Smart Campaign中编辑资格规则 — Marketo文档 — 产品文档
title: 在智能营销活动中编辑资格规则
exl-id: 8b016fe4-8caf-4266-9f8f-2b05dae78cff
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# 在智能营销活动中编辑资格规则 {#edit-qualification-rules-in-a-smart-campaign}

资格规则可控制某人在智能营销活动中流过的次数。 默认情况下，即使有人多次触发智能营销活动，也只能通过流量发送一次。 下面是如何修改这些设置的。

1. 在智能营销策划中，单击 **计划** 选项卡，然后 **编辑设置**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign-1.png)

   >[!TIP]
   >
   >您还可以单击 **编辑** “Smart Campaign设置”右侧。

1. 选择通过智能营销活动流运行人员的频率： **仅一次**， **每次**，或 **每#天一次**/**周**/**月**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >如果每天设置一次规则，Marketo会将该规则转换为小时数。 例如，如果您将规则设置为每天一次，而某个人在星期日夜间的晚上10点符合条件，则直到星期一夜间的晚上10点才能再次符合条件。 使用周或月时，此逻辑也适用。 一个月始终计为30天。

   >[!NOTE]
   >
   >默认情况下，通信限制不适用于智能营销活动。 了解如何 [将通信限制应用于智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md).

   >[!NOTE]
   >
   >[将通信限制应用于智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md)

任务完成了！ 您现在知道如何在智能营销活动中控制资格规则。
