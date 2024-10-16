---
description: 了解电子邮件步骤的Sales Campaign发送选项 — Marketo文档 — 产品文档
title: 了解电子邮件步骤的Sales Campaign发送选项
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 832635c9e029754ce094e4137724bcc956dbcd35
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 了解电子邮件步骤的Sales Campaign发送选项 {#understanding-sales-campaign-send-options-for-email-steps}

在创建销售活动时，对于如何在Sales Insight Actions中创建电子邮件步骤，您有多个选项。 而且，根据电子邮件在促销活动中的位置，您的选项也会有所不同。

## 第一步发送选项 {#first-step-send-options}

如果这是您的第一个步骤，并且是促销活动的第一天，您将可以选择以下选项：

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### 我将选择发送此电子邮件的时间 {#first-step-i-will-choose}

* 通过此选项，当您通过添加人员来启动促销活动时，可以为促销活动中的第一封电子邮件选择“发送时间”时间。

### 请在以下时间发送此电子邮件 {#first-step-following-time}

* 当您通过向促销活动添加人员来启动促销活动时，我们将计划此时发送电子邮件。
* 您始终可以选择在开始促销活动时选择新的“发送时间”。

### 创建任务；我将自己发送此电子邮件 {#first-step-create-a-task}

* 此选项将创建一个电子邮件任务(并同步到Salesforce)，您可以在方便时发送该任务。
* 作出此选择后，当您启动销售活动时，我们将在指挥中心和实时信息源中为您将这些任务排入队列。 然后，您可以个性化并发送（或计划）每封电子邮件，然后再发送。

   * 如果您在Web应用程序中打开此任务，它将打开一个撰写窗口，其中包含联系人的电子邮件地址、电子邮件的主题行以及您选择的模板。
   * 如果在Gmail或Outlook中打开此任务，它将打开本机撰写窗口，并动态填充联系人的电子邮件地址、电子邮件的主题行以及您选择的模板。

## 后续步骤发送选项 {#subsequent-step-send-options}

对于Sales Campaign中的任何后续日期/步骤，您将具有以下选项：

### 与此销售活动中的上一封电子邮件同时发送此电子邮件 {#subsequent-send-at-same-time}

* 此选项将在电子邮件直接之前与电子邮件同时发送电子邮件。
* 在关联的日期仍会发送。

>[!IMPORTANT]
>
>同一天发送的电子邮件不支持与上一封电子邮件同时发送电子邮件。 相反，将在发送前一天发送的电子邮件时发送电子邮件。 如果为营销活动第一天的电子邮件选择了此选项（不推荐），则会在营销活动开始时立即发送该电子邮件。

### 请在以下时间发送此电子邮件 {#subsequent-send-at-following-time}

* 当您通过向促销活动添加人员来启动促销活动时，我们将计划此时发送电子邮件。
* 您始终可以选择在开始促销活动时选择新的“发送时间”。

### 创建任务；我将自己发送此电子邮件 {#subsequent-create-a-task}

* 此选项将创建一个电子邮件任务(并同步到Salesforce)，您可以在方便时发送该任务。
* 作出此选择后，当您启动销售促销活动时，销售分析操作将在指挥中心和实时信息源中为您排列这些任务。 然后，您可以个性化并发送（或计划）每封电子邮件，然后再发送。

   * 如果您在Web应用程序中打开此任务，它将打开一个撰写窗口，其中包含联系人的电子邮件地址、电子邮件的主题行以及您选择的模板。
   * 如果在Gmail或Outlook中打开此任务，它将打开本机撰写窗口，并动态填充联系人的电子邮件地址、电子邮件的主题行以及您选择的模板。

### 创建此电子邮件作为此营销活动中上一封电子邮件的跟进 {#subsequent-create-this-email}

* 如果您希望将销售活动中的上一封电子邮件附加到销售活动发送的下一封电子邮件，请启用此复选框。
* 对于电子邮件的附加副本，将始终发送销售活动中的电子邮件模板。 用户在发出之前所做的任何编辑都不会包含在发送中。

>[!NOTE]
>
>用于创建电子邮件作为后续的选项将仅在电子邮件步骤中可用，前提是前一步也是电子邮件。 如果上一步是“调用”、“InMail”或“自定义”，则不会显示创建跟进操作的选项。

>[!MORELIKETHIS]
>
>[创建促销活动](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>[销售活动步骤类型和提醒任务](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>[Sales Campaign设置](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}

