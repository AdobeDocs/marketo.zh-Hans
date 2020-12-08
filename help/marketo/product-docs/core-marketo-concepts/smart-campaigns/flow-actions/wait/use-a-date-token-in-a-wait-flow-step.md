---
unique-page-id: 1146997
description: 在等待流程步骤- Marketo Docs —— 产品文档中使用日期令牌
title: 在等待流步骤中使用日期令牌
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 在等待流步骤中使用日期令牌 {#use-a-date-token-in-a-wait-flow-step}

您可以使用等待流程步骤暂停人员在智能活动中的旅程，直到使用日期令牌的特定日期为止。 您还可以按天数修改结束日期。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>这仅适用于触发活动。 无法在批处理活动中使用此功能。

1. 在智能活动 **流** 选项卡中，拖 **动等待** 流步骤。

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. 单击右侧的齿轮图标。

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. 从“类 **型** ”下拉菜单中，选 **择日期令牌**。

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
   >您还可以使用表示整数字段或 `{{lead.` 数字 `{{company.` 类型的标记来指定 `{{my.` 天数或标记。

1. 单击“保存”。

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**相关文章**
   >
   >* [在等待流步骤中使用持续时间](use-a-duration-in-a-wait-flow-step.md)
   >* [在等待流程步骤中使用特定日期](use-a-specific-date-in-a-wait-flow-step.md)


