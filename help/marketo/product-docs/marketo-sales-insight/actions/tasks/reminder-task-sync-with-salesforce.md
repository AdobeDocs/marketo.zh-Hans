---
description: 与Salesforce同步提醒任务 — Marketo文档 — 产品文档
title: 提醒任务与 Salesforce 同步
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# 与[!DNL Salesforce]同步的提醒任务 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>要了解如何启用任务同步，请签出[将销售Insight操作任务/提醒同步到Salesforce任务](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks)。

启用任务同步设置后，用户将看到他们的提醒任务与[!DNL Salesforce]双向同步。 这意味着用户可以从[!DNL Salesforce]或[!DNL Sales Insight Actions]中管理任务，并且确信系统将保持一致性。

## 提醒任务字段同步 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下是[!DNL Sales Insight Actions]中的提醒任务字段及其通过双向任务同步支持的相应[!DNL Salesforce]字段的列表。

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] 任务字段</th>
  <th>[!DNL Salesforce] 任务字段</th>
  <th>[!DNL Salesforce] 任务</th>
 </tr>
 <tr>
  <td>[!UICONTROL Task Name]</td>
  <td>[!UICONTROL Subject Field]</td>
  <td>简短摘要字段，用于显示任务的标题。</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Task Status]</td>
  <td><p>显示任务的状态。 [!DNL Sales Insight Actions]任务有两个状态，这些状态映射到[!DNL Salesforce]任务状态选取列表中的两个值。</p>
  <p>在[!DNL Sales Insight Actions]中打开=未在[!DNL Salesforce]中启动。</p>
  <p>在[!DNL Sales Insight Actions]内完成=在[!DNL Salesforce]内完成。</p>
  <p>[!DNL Salesforce]中的其他状态值将不会同步到[!DNL Sales Insight Actions]。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Priority]</td>
  <td>[!UICONTROL Priority]</td>
  <td><p>[!DNL Sales Insight Actions] 优先级可以是“正常”或“高”，它们映射到[!DNL Salesforce]中的“正常”和“高”优先级值。</p>
  <p>[!DNL Salesforce]中的低优先级值将不会同步到[!DNL Sales Insight Actions]。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Due Date]</td>
  <td>[!UICONTROL Due Date]</td>
  <td>任务的截止日期。</td>
 </tr>
 <tr>
  <td>[!UICONTROL Details]</td>
  <td>[!UICONTROL Comments]</td>
  <td>显示有关应该使用提醒任务完成的内容的更多详细信息。</td>
 </tr>
</table>

## 首次将[!DNL Sales Insight Actions]任务与[!DNL Salesforce]同步 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

当您首次打开[!DNL Sales Insight Actions]和[!DNL Salesforce]任务之间的同步时，我们会导入您的[!DNL Salesforce]任务。 我们&#x200B;**不会**&#x200B;将您在[!DNL Sales Insight Actions]中拥有的任何当前任务推送到[!DNL Salesforce]。 为了减少待处理内容和重复项，从[!DNL Sales Insight Actions]同步到[!DNL Salesforce]的任务只有在&#x200B;*之后您将*&#x200B;与SFDC同步的[!DNL Sales Insight Actions]创建的任务。

以下是同步[!DNL Sales Insight Actions]和SFDC任务时发生的情况：

* 在同步的任务上单击“保存”后，它们就会开始进行同步。 这最初将需要一些时间。

* 过去24小时内已更新或创建的任何提醒都将从SFDC拉入[!DNL Sales Insight Actions]。 同步基于到期日期，所有这些任务将在后端进行同步，但在命令中心，您只能看到今天和明天到期的任务。

* 如果以前启用了同步，并且您删除了SFDC中的任何任务，则过去15天内删除的任何任务都将从命令中心删除。

* 只要已启用同步，我们就会一直在[!DNL Sales Insight Actions]和SFDC之间同步任务。

初始同步后，您在[!DNL Sales Insight Actions]中创建、编辑、完成或删除的任何任务都将同步到[!DNL Salesforce]中的任务列表。 在[!DNL Salesforce]中创建、编辑、完成或删除的任何内容都将在[!DNL Sales Insight Actions]中更新您的任务列表。

若要启用此同步，只需在Web应用程序的[设置页面](https://toutapp.com/login)中选中同步框即可。

>[!NOTE]
>
>任务的主题字段可以在[!DNL Sales Insight Actions]中更新，并且如果正在使用[!DNL Salesforce]活动详细信息自定义`{{activity_subject}}`设置中的[动态字段，则该更新将在相应同步任务的](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md)主题字段中同步。 相反，对[!DNL Salesforce]中的主题字段所做的任何更新将&#x200B;*不会*&#x200B;同步到[!DNL Sales Insight Actions]提醒任务主题字段。
