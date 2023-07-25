---
unique-page-id: 1146997
description: 在等待流步骤中使用日期令牌 — Marketo文档 — 产品文档
title: 在等待流步骤中使用日期令牌
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 在等待流步骤中使用日期令牌 {#use-a-date-token-in-a-wait-flow-step}

您可以使用等待流量步骤暂停人员通过智能营销活动的历程，直到使用日期令牌的特定日期为止。 您还可以将结束日期修改若干天。

>[!NOTE]
>
>这仅适用于触发营销活动。 您无法在批量营销活动中使用此功能。

1. 在您的智能营销活动中 **流量** 选项卡，拖动到 **等待** 流程步骤。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 单击右侧的齿轮图标。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 从 **类型** 下拉列表，选择 **日期令牌**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 选择一个日期令牌，以指定等待步骤的结束时间：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 要等到当前日历年或下一个日历年出现日期的下一个周年，请选中该框。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >在引用过去日期（如生日或合同开始日期）的日期令牌上使用此选项。

1. （可选）您可以按指定的天数修改终止日期。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >您还可以使用指定天数 `{{lead.` 或 `{{company.` 表示整数字段的令牌，或 `{{my.` 数字类型的令牌。

1. 单击 **保存**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
