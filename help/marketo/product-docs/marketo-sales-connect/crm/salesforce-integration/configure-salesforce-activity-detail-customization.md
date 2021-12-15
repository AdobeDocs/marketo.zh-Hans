---
description: 配置Salesforce活动详细信息自定义 — Marketo文档 — 产品文档
title: 配置Salesforce活动详细信息自定义
hide: true
hidefromtoc: true
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: 87f43fb58b5739c0465a1a74fb60cdf5c5f6b759
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 配置Salesforce活动详细信息自定义 {#configure-salesforce-activity-detail-customization}

活动详细信息自定义允许管理员配置在将Salesforce活动/提醒任务同步到Salesforce时，将记录到Salesforce任务 — 主题字段的信息。

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

该功能可用于释放以下优势：

* 通过自定义在主题字段上显示哪些信息，可轻松扫描Salesforce中销售的活动详细信息。
* 管理员可以使用唯一标识符（如“Mkto_sales”）标记主题字段，以便能够轻松识别Sales Connect中的活动，并将其与其他电子邮件活动、呼叫活动和任务区分开来。
* 无需自定义活动字段。 Salesforce对自定义活动字段的数量实施限制，这可以限制可在报表中使用的数据。 通过使用活动动态字段向主题行添加关键数据，您可以减少在Salesforce实例中创建所需的自定义活动字段数。
* 活动和任务的主题字段将遵循Sales Connect管理员定义的一致模式。

## 支持的活动动态字段 {#activity-dynamic-fields-supported}

活动动态字段引用有关销售活动的信息以填充数据。 现在，它们可以与Salesforce活动详细信息自定义一起使用。

>[!NOTE]
>
>如果没有值来填充特定活动/任务的动态字段，则在更新Salesforce任务 — 主题字段时，不会填充该动态字段的任何数据。

<table>
 <tr>
  <th>字段</th>
  <th>描述</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>将以“电子邮件”、“呼叫”、“InMail”或“自定义”填充任务类型。</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>将填充任务的主题。</p>
      <p>对于电子邮件，将填充电子邮件的主题行。</p>
      <p>对于调用、inMail或自定义，如果在任务名称/主题字段中创建了具有值的提醒任务，则将填充一个值。</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>如果活动是从销售活动发起的，则会填充销售活动的名称。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>如果活动是从销售活动发起的，它将填充此活动发生的销售活动日编号。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>如果活动是从销售活动启动的，它将在此活动发生的销售活动日期内填充步骤号。</td>
 </tr>
 <tr>
  <td>{{call_oupt}}</td>
  <td>如果活动是调用，并且选择了调用结果，则将填充调用结果值。</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>如果活动是调用，并且选择了调用原因，则会填充调用原因值。</td>
 </tr>
</table>

## 配置Salesforce活动详细信息自定义 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**需要管理员权限。**

在配置活动详细信息时，请考虑在Salesforce中查看任务历史记录时哪些数据与销售最相关。

1. 单击齿轮图标，然后选择 **设置**.

PICC

1. 单击 **Salesforce**.

PICC

1. 单击 **同步设置**.

PICC

1. 在活动详细信息自定义编辑器中，添加您需要的任何自由文本，对于同步到Salesforce的所有任务的主题字段，此文本将保持不变。

1. 通过单击动态字段按钮并从列表中选择要使用的动态字段，可添加要添加的任何动态字段。

1. 单击 **保存**.

>[!NOTE]
>
>Salesforce强制规定255个字符的限制。 如果活动详细信息超过该值，则将被截断，以确保该信息可以存储在Salesforce主题字段中。

>[!MORELIKETHIS]
>
>* [同步设置](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [提醒任务与Salesforce同步](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [针对CRM的Sales Connect自定义](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
