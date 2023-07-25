---
description: 将致电原因和致电结果记录到Salesforce - Marketo文档 — 产品文档
title: 将致电原因和致电结果记录到Salesforce
exl-id: cfe71388-282b-45e5-a817-45a951f613bc
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 将致电原因和致电结果记录到Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

如果您出于报告或可见性的目的，希望将致电结果记录并致电原因发送到Salesforce，则可以为每个创建自定义活动字段。 每个字段都必须使用特定的API名称（在Salesforce中称为“字段名称”）。

* 呼叫结果字段名称：mktosales_call_outcome
* 致电原因字段名称：mktosales_call_reason

要利用这些字段，您首先需要将字段创建为自定义活动字段。 为了使其对用户可见，您需要将其添加到任务对象页面布局。

## Salesforce Classic {#salesforce-classic}

### 在Salesforce Classic中创建自定义活动字段  {#create-custom-activity-field-in-salesforce-classic}

1. 在Salesforce中，单击 **设置**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. 在“快速查找”框中键入“Activities”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. 单击 **活动自定义字段**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. 单击 **新**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. 选择数据类型“文本”并单击 **下一个**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. 为自定义字段提供上面定义的字段名称。 字段长度限制为255个字符。 字段标签将是您的销售团队可见的字段，并且可以根据您团队的需求进行自定义。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. 其余设置是可选的。 完成配置后，单击 **下一个**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. 为此字段选择所需的字段级安全设置，然后单击 **下一个** （下图只是一个示例）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >确保自定义字段对Sales Insight Actions用户使用的用户档案可见，以及您希望其可见的任何其他位置均可见。

1. 选择要将该字段添加到的页面布局，然后单击 **保存** （可选）您可以单击 **保存并新建** 并对“来电原因”字段重复此过程)。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### 在Salesforce Classic中向任务页面布局添加自定义活动字段 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>如果您没有在上面的步骤9中选择所需的页面布局，则您只需执行以下步骤即可。

1. 在Salesforce中，单击 **设置**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. 在“快速查找”框中键入“Task”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. 单击 **任务页面布局**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. 单击 **编辑** 在要添加此字段的任务页面布局旁边。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. 将字段拖放到任务页面布局的所需部分。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. 单击 **保存**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### 在Salesforce Lightning中创建自定义活动字段 {#create-custom-activity-field-in-salesforce-lightning}

1. 在Salesforce中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. 单击 **对象管理器**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. 在“快速查找”框中键入“Activity”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. 单击 **活动** 标签。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. 单击 **字段和关系**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. 单击 **新**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### 在Salesforce Lightning中将自定义活动字段添加到任务页面布局 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. 在Salesforce中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. 单击 **对象管理器**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. 在“快速查找”框中键入“Task”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. 单击 **任务** 标签。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. 单击 **页面布局**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. 单击您想要将此字段添加到的任务页面布局。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. 将字段拖放到任务页面布局的所需部分。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. 单击 **保存**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>* [调用结果](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-outcomes.md)
>* [致电原因](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-reasons.md)
