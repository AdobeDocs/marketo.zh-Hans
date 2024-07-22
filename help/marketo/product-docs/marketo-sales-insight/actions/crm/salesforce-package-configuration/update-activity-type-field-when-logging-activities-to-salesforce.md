---
description: 将活动记录到Salesforce时更新Activity Type字段 — Marketo文档 — 产品文档
title: 将活动记录到Salesforce时更新Activity Type字段
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 1%

---

# 将活动记录到Salesforce时更新Activity Type字段 {#update-activity-type-field-when-logging-activities-to-salesforce}

操作可以自动将您的电子邮件和调用活动同步到Salesforce以用于报告并提高活动历史记录的可见性。 在记录活动时，请确保根据所记录的活动类型，将“活动类型”字段正确更新为“电子邮件”、“呼叫”或“回复”。

>[!NOTE]
>
>通过密件抄送记录电子邮件时，不会查找“任务类型”选取列表，而是会自动将“类型”字段填充为“电子邮件”，因为它们将通过您的密件抄送地址传送到Salesforce。

## 注意事项 {#things-to-know}

* 需要与Salesforce建立连接，任务类型才能更新。
* 任务类型选择列表中不应选择默认类型值。
* “呼叫”、“回复”和“电子邮件”都必须存在于“任务类型”选取列表中（大写问题）。
* Salesforce中更新任务类型字段的工作流或触发器可能会干扰此过程。

## 设置 {#setup}

首先检查您是否已设置正确的选取列表值。 您需要Salesforce管理员的帮助才能对选择列表进行任何更改。

首先检查您的任务类型选择列表（电子邮件、呼叫和回复中）中缺少哪些值。 您可能需要Salesforce管理员的帮助才能查看此信息并对活动类型选取列表进行更改。 要进行这些更改，您的Salesforce管理员可以执行以下步骤。

### 在Salesforce Lightning中 {#salesforce-lightning}

1. 导航到[Salesforce.com](https://salesforce.com){target="_blank"}。
1. 单击右上角的齿轮图标，然后选择&#x200B;**设置** > **对象管理器**。
1. 在“快速查找”框中键入“task”。
1. 在左侧面板中，单击&#x200B;**字段和关系**。
1. 单击字段标签&#x200B;**类型**。
1. 在任务类型选择列表值下，单击&#x200B;**新建**。
1. 键入缺少的任务类型选择列表值的名称（“电子邮件”、“呼叫”、“回复”）。
1. 单击&#x200B;**保存**。

### 在Salesforce Classic中 {#salesforce-classic}

1. 导航到[Salesforce.com](https://salesforce.com){target="_blank"}。
1. 单击&#x200B;**设置** > **生成** > **自定义** > **活动** > **任务字段**。
1. 单击&#x200B;**类型**。
1. 在任务类型选择列表值下，单击&#x200B;**新建**。
1. 键入缺少的任务类型选择列表值的名称（“电子邮件”、“呼叫”、“回复”）。
1. 单击&#x200B;**保存**。

现在，您已设置好，接下来会看到类型字段填充了记录的电子邮件、呼叫和回复的相应值。 这些值将&#x200B;_不在_&#x200B;销售分析操作提醒任务中填充。

>[!NOTE]
>
>如果您未看到“回复”作为值，请单击&#x200B;**新建**&#x200B;以添加它。 “回复”不是Salesforce中的标准值。

>[!MORELIKETHIS]
>
>* [将销售活动属性记录到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [配置Salesforce活动详细信息自定义](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [将销售活动同步到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
