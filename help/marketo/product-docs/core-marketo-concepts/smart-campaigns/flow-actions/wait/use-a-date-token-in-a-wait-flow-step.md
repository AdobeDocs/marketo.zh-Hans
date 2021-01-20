---
unique-page-id: 1146997
description: 在等待流程步骤- Marketo Docs —— 产品文档中使用日期令牌
title: 在等待流步骤中使用日期令牌
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 在等待流步骤{#use-a-date-token-in-a-wait-flow-step}中使用日期令牌

您可以使用等待流程步骤暂停人员在智能活动中的旅程，直到使用日期令牌的特定日期为止。 您还可以按天数修改结束日期。

>[!NOTE]
>
>这仅适用于触发活动。 无法在批处理活动中使用此功能。

1. 在智能活动&#x200B;**流**&#x200B;选项卡中，拖动到&#x200B;**等待**&#x200B;流步骤上。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 单击右侧的齿轮图标。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 从&#x200B;**类型**&#x200B;下拉列表中，选择&#x200B;**日期令牌**。

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. 选择日期令牌以指定等待步骤何时结束：

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. 要等到当前或下一个日历年中日期的下一个周年，请选中此复选框。

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >在日期令牌中使用此选项，日期令牌是指过去的日期，如生日或合同开始日期。

1. （可选）您可以按指定的天数修改结束日期。

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >您还可以使用表示整数字段的`{{lead.`或`{{company.`令牌或数字类型的`{{my.`令牌指定天数。

1. 单击&#x200B;**保存**。

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [在等待流步骤中使用持续时间](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步骤中使用特定日期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

