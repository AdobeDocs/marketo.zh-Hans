---
unique-page-id: 1146997
description: 在等待流步骤中使用日期令牌 — Marketo文档 — 产品文档
title: 在等待流步骤中使用日期令牌
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 在等待流步骤中使用日期令牌 {#use-a-date-token-in-a-wait-flow-step}

您可以使用等待流步骤暂停人员通过智能营销活动的历程，直到使用日期令牌的特定日期为止。 您还可以将结束日期修改若干天。

>[!NOTE]
>
>这仅适用于触发营销活动。 您无法在“批处理营销活动”中使用此功能。

1. 在Smart Campaign **[!UICONTROL Flow]**&#x200B;选项卡中，拖动&#x200B;**[!UICONTROL Wait]**&#x200B;流程步骤。

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. 单击齿轮图标。

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. 从&#x200B;**[!UICONTROL Type]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Date Token]**。

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. 选择一个[!UICONTROL Date token]以指定等待步骤的结束时间：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. 要等到当前日历年或下一个日历年出现该日期的下一个周年，请选中该框。

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >在引用过去日期（如生日或合同开始日期）的日期令牌上使用此选项。

1. （可选）您可以按指定的天数修改终止日期。

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >您还可以使用表示整数字段的`{{lead.`或`{{company.`令牌或数字类型的`{{my.`令牌指定天数。

1. 单击 **[!UICONTROL Save]**。

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}中使用持续时间
   >* [在等待流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}中使用特定日期
