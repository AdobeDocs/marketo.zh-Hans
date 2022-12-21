---
unique-page-id: 1146974
description: 在智能营销活动中编辑资格规则 — Marketo文档 — 产品文档
title: 在智能营销活动中编辑资格规则
exl-id: 8b016fe4-8caf-4266-9f8f-2b05dae78cff
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# 在智能营销活动中编辑资格规则 {#edit-qualification-rules-in-a-smart-campaign}

资格规则控制某个人在智能营销活动中可以运行流程的次数。 默认情况下，即使某人多次触发智能营销活动，他们也只会通过流程发送一次。 以下是如何修改这些设置。

1. 在您的智能营销活动中，单击 **计划** 选项卡，然后 **编辑设置**.

   ![](assets/programeditsettings-hands.png)

   >[!TIP]
   >
   >您还可以单击 **编辑** 右侧的“智能营销活动设置”。

1. 选择通过智能营销活动流程来引导用户的频率： **仅一次**, **每次**&#x200B;或 **每天**/**周**/**月**.

   ![](assets/edit-qualification-rules-in-a-smart-campaign.png)

   >[!NOTE]
   >
   >每天设置一次规则时，Marketo会将该规则转换为小时。 例如，如果将规则设置为每天一次，而某人在周日晚上10点符合条件，则该人员在周一晚上10点之前无法再次符合条件。 此逻辑在使用周或月时也适用。 一个月始终被计为30天。

   >[!NOTE]
   >
   >默认情况下，通信限制不会应用于智能营销活动。 了解如何 [对智能营销活动应用通信限制](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md).

   >[!NOTE]
   >
   >[将通信限制应用于智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/apply-communication-limits-to-smart-campaign.md)

任务完成！ 您现在知道如何在智能营销活动中控制资格规则。
