---
description: 将活动记录到Salesforce时更新活动类型字段 — Marketo文档 — 产品文档
title: 将活动记录到Salesforce时更新活动类型字段
exl-id: f65d7d97-ec65-4210-9381-02be788498f9
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 将活动记录到Salesforce时更新活动类型字段 {#update-activity-type-field-when-logging-activities-to-salesforce}

操作可以自动将您的电子邮件和呼叫活动同步到Salesforce以用于报告，并提高活动历史记录的可见性。 在记录活动时，请确保根据所记录的活动类型，将“活动类型”字段正确更新为“电子邮件”、“呼叫”或“回复”。

>[!NOTE]
>
>通过密件抄送记录电子邮件不会查看“任务类型”选取列表，而是会自动将“类型”字段填充为“电子邮件”，因为它们将通过您的密件抄送地址传送到Salesforce。

## 注意事项 {#things-to-know}

* 需要与Salesforce建立连接才能更新任务类型。
* 任务类型选择列表中不应选择默认类型值。
* “任务类型”选择列表中必须存在“呼叫”、“回复”和“电子邮件”（大写内容）。
* Salesforce中更新任务类型字段的工作流或触发器可能会干扰此过程。

## 设置 {#setup}

首先检查您是否已设置正确的选取列表值。 您需要Salesforce管理员的帮助才能对选择列表进行任何更改。

首先检查您的任务类型选择列表（电子邮件、呼叫和回复中）中缺少哪些值。 您可能需要Salesforce管理员的帮助来查看此信息，并对活动类型选取列表进行更改。 要进行这些更改，您的Salesforce管理员可以执行以下步骤。

### Salesforce Lightning内容 {#salesforce-lightning}

1. 导航到 [Salesforce.com](https://salesforce.com){target="_blank"}.
1. 单击右上角的齿轮图标，然后选择 **设置** > **对象管理器**.
1. 在“快速查找”框中键入“task”。
1. 在左侧面板中，单击 **字段和关系**.
1. 单击字段标签 **类型**.
1. 在任务类型选择列表值下，单击 **新**.
1. 键入缺少的任务类型选择列表值的名称（“电子邮件”、“调用”、“回复”）。
1. 单击 **保存**.

### 在Salesforce Classic中 {#salesforce-classic}

1. 导航到 [Salesforce.com](https://salesforce.com){target="_blank"}.
1. 单击 **设置** > **生成** > **自定义** > **活动** > **任务字段**.
1. 单击 **类型**.
1. 在任务类型选择列表值下，单击 **新**.
1. 键入缺少的任务类型选择列表值的名称（“电子邮件”、“调用”、“回复”）。
1. 单击 **保存**.

现在，设置完此选项后，您将看到类型字段填充了记录的电子邮件、呼叫和回复的相应值。 这些值将 _非_ 在销售分析操作提醒任务中填充。

>[!NOTE]
>
>如果您未看到“回复”作为值，请单击以添加它 **新**. “Reply”不是Salesforce中的标准值。

>[!MORELIKETHIS]
>
>* [将销售活动属性记录到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [配置Salesforce活动详细信息自定义](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [将Sales Activities同步到Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
