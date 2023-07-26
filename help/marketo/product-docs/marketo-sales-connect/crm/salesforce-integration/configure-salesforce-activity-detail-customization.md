---
description: 配置Salesforce活动详细信息自定义 — Marketo文档 — 产品文档
title: 配置Salesforce活动详细信息自定义
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# 配置Salesforce活动详细信息自定义 {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce和Marketo Sales Connect [必须连接](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* 通过API记录电子邮件活动 [必须启用](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)

活动详细信息自定义允许管理员配置在Sales Connect活动/提醒任务同步到Salesforce时记录到Salesforce Task - Subject Field的信息。

>[!NOTE]
>
>* 如果您使用的是，对提醒任务的Sales Connect主题字段所做的更新将反映在对应Salesforce任务的主题字段中 `{{activity_subject}}` 活动详细信息自定义中的动态字段。
>* 将信息记录到Salesforce主题字段时不支持换行符。 更新销售任务主题时，将删除活动详细信息自定义编辑器中的任何换行符。

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>InMail提醒任务</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>电子邮件活动</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>调用活动</td>
 </tr>
</table>

此功能可用于解锁以下优势：

* 通过自定义在主题字段中可见的信息，可以轻松地在Salesforce中扫描销售活动的详细信息。
* 管理员可以使用唯一标识符（如“Mkto_sales”）标记subject字段，以便可以轻松地识别Sales Connect中的活动，并将其与其他电子邮件活动、呼叫活动和任务区分开来。
* 减少对自定义活动字段的需求。 Salesforce对自定义活动字段的数量实施限制，从而限制可在报表中使用的数据。 通过使用活动动态字段将关键数据添加到主题行，您可以减少需要在Salesforce实例中创建的自定义活动字段的数量。
* 活动和任务的主题字段将遵循Sales Connect管理员定义的一致模式。

>[!NOTE]
>
>如果您将电子邮件回复作为活动记录到Salesforce，则不会使用Salesforce活动详细信息自定义设置。 相反，他们将记录为“回复：电子邮件主题”。

## 支持的活动动态字段 {#activity-dynamic-fields-supported}

活动动态字段引用有关销售活动的信息以填充数据。 现在，它们可以与Salesforce活动详细信息自定义一起使用。

>[!NOTE]
>
>如果没有值来填充特定活动/任务的动态字段，那么在更新Salesforce任务 — 主题字段时，它将不会填充该动态字段的任何数据。

<table>
 <tr>
  <th>字段</th>
  <th>描述</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>将填充任务类型，如Email、Call、InMail或Custom。</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>将填充任务的主题。</p>
      <p>如果是电子邮件，则会填充电子邮件的主题行。</p>
      <p>在调用、inMail或自定义的案例中，如果创建了一个提醒任务，且该任务名称/主题字段中有值，则系统会填充一个值。</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>如果活动是从销售活动发起的，则会填充销售活动的名称。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>如果活动是从销售市场活动启动的，则会填充此活动发生的销售市场活动日期编号。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>如果活动是从销售市场活动启动的，则会填充此活动发生的销售市场活动日期内的步骤编号。</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>如果活动是调用并且选择了调用结果，则会填充调用结果值。</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>如果活动是呼叫并且选择了呼叫原因，则会填充呼叫原因值。</td>
 </tr>
</table>

## 配置Salesforce活动详细信息自定义 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**需要管理员权限。**

在配置活动详细信息时，请考虑在Salesforce中查看任务历史记录时哪些数据与销售最相关。

1. 单击齿轮图标并选择 **设置**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. 单击 **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. 单击 **同步设置**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. 在活动详细信息自定义编辑器中，添加所需的任意自由文本。 您添加的文本是非动态的，对于同步到Salesforce的所有任务的subject字段将保持不变。

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >尽管不是必需的，但将添加的文本换行到直括号中可以让某些人在数据填充到Salesforce中的主题字段时更容易识别这些数据。 示例： `[Sales Connect] - {{Activity_type}}`

1. 通过单击 **添加动态字段** 按钮。

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. 选择所需的动态字段。

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. 单击 **保存**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce强制执行255个字符的限制。 如果您的活动详细信息超出此范围，则将截断以确保信息存储在Salesforce主题字段中。

>[!MORELIKETHIS]
>
>* [同步设置](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [与Salesforce同步提醒任务](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [CRM的Sales Connect自定义](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
