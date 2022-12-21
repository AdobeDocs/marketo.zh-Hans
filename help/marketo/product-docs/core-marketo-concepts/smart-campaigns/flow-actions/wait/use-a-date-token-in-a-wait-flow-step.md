---
unique-page-id: 1146997
description: 在等待流程步骤中使用日期令牌 — Marketo文档 — 产品文档
title: 在等待流程步骤中使用日期令牌
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# 在等待流程步骤中使用日期令牌 {#use-a-date-token-in-a-wait-flow-step}

您可以使用等待流程步骤暂停人员在智能营销活动中的历程，直到使用日期令牌的特定日期为止。 您还可以按某些天数修改结束日期。

>[!NOTE]
>
>这仅适用于触发营销活动。 您无法在批量营销活动中使用此功能。

1. 在您的智能营销活动中 **流量** 选项卡 **等待** 流步骤。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 单击右侧的齿轮图标。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 从 **类型** 下拉列表，选择 **日期令牌**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 选择日期令牌以指定等待步骤应在何时结束：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 要等到当前或下一个日历年中出现日期的下一个周年，请勾选方框。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >在日期令牌中使用此选项，这些令牌表示过去的日期，如生日或合同开始日期。

1. （可选）您可以按指定的天数修改结束日期。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >您还可以使用 `{{lead.` 或 `{{company.` 表示整数字段或 `{{my.` 数字类型的令牌。

1. 单击 **保存**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流程步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

