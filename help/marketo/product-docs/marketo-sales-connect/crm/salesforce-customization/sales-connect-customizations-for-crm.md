---
unique-page-id: 14745793
description: CRM的Sales Connect自定义 — Marketo文档 — 产品文档
title: CRM的Sales Connect自定义
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
source-git-commit: 94f89e64b69d3997effe6736241a68f8314db1e6
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# CRM的Sales Connect自定义 {#sales-connect-customizations-for-crm}

以下字段和按钮由Salesforce CRM中的元数据API创建。 创建字段后，管理员必须在其CRM中配置页面布局以显示它们。 有关说明，请参阅 [此处](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>这会影响ToutApp和Sales Connect客户。

## 如何在Salesforce中安装自定义项 {#how-to-install-customizations-in-salesforce}

1. 在Sales Connect中，单击齿轮图标，然后选择 **设置**.

   ![](assets/one.png)

1. 在“管理员设置”下，选择 **Salesforce**.

   ![](assets/two.png)

1. 单击 **Marketo Sales Connect自定义**.

   ![](assets/three.png)

1. 单击 **连接到Salesforce**.

   ![](assets/four.png)

1. 登录到Salesforce。

   ![](assets/five.png)

## 更新Salesforce自定义 {#update-salesforce-customization}

对Salesforce自定义包的更新将包括增强功能和错误修复。 要检查更新是否可用或是否执行更新，请执行以下步骤。

>[!NOTE]
>
>**需要管理员权限。**

1. 在 [Web应用程序](https://www.toutapp.com)，请单击齿轮图标并选择 **设置**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. 在“管理员设置”下，单击 **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Sales Connect自定义卡片将显示是否有更新。 单击 **更新自定义**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. 单击 **升级**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. 等待更新安装。 安装时间将因您需要的版本号而异。

   ![](assets/sales-connect-customizations-for-crm-10.png)

完成后，您的卡片将显示“Your Sales Connect自定义项是最新的。”

![](assets/sales-connect-customizations-for-crm-11.png)

## 自定义活动字段 {#custom-activity-fields}

Marketo将检测到新字段的创建情况，然后对数据进行一次性回填、重新映射，并持续将值同步到 **新建** 字段。 旧字段将不会更新。

| **字段名称** | **描述** |
|---|---|
| MSE调用本地存在ID | 作为用户，当您从MSE Phone发出呼叫时，可以选择“本地存在”作为一个选项。 来电将显示接收器的本地号码。 |
| MSE调用记录URL | 可以在此处记录调用，并记录该录制的链接。 |
| MSE营销活动 | 联系人/潜在客户所属的MSE营销活动的日志名称。 |
| MSE促销活动URL | 将URL记录到在MSE中创建的营销活动。 单击此按钮将在MSE Web应用程序中打开营销活动。 |
| MSE促销活动当前步骤 | 如果联系人/潜在客户是营销活动的一部分，则此字段将记录潜在客户/联系人当前所在步骤的名称。 |
| 已查看MSE电子邮件附件 | 在随附件发送电子邮件且收件人查看附件时，记录数据。 |
| 已点击MSE电子邮件 | 当收件人单击电子邮件中的链接时，会记录一个复选标记。 |
| MSE电子邮件已回复 | 收件人回复电子邮件时记录复选标记。 |
| MSE电子邮件状态 | 显示是否发送/进行中/退回电子邮件（跟踪弹回的电子邮件取决于使用的投放渠道）。 |
| MSE电子邮件模板 | 在发送给潜在客户/联系人的电子邮件中使用的MSE模板的日志名称。 |
| MSE电子邮件模板URL | 将URL记录到在MSE中创建的模板。 单击此按钮将在MSE Web应用程序中打开模板。 |
| MSE电子邮件URL | 单击此URL将在MSE中打开命令中心，并拉出“人员详细信息视图”历史记录选项卡，在该选项卡中可以查看已发送的电子邮件。 |
| 已查看的MSE电子邮件 | 收件人查看电子邮件时记录复选标记。 |

## 汇总日志记录字段 {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>字段名称</strong></td> 
   <td><strong>描述</strong></td> 
  </tr> 
  <tr> 
   <td>MSE — 上次营销参与</td> 
   <td>上次从营销传入的参与。 </td> 
  </tr> 
  <tr> 
   <td>MSE — 上次营销参与日期</td> 
   <td>营销活动参与的时间戳。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上次营销参与度设计</td> 
   <td>项目描述。</td> 
  </tr> 
  <tr> 
   <td>MSE — 上一个营销参与来源</td> 
   <td>营销参与度来源。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次营销参与类型</td> 
   <td colspan="1">参与度类型。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 按销售列出的上一个活动<br></td> 
   <td colspan="1">销售团队执行的上次传出活动。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次答复</td> 
   <td colspan="1">对销售电子邮件的上次电子邮件回复。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 当前销售活动</td> 
   <td colspan="1">潜在客户/联系人所属的MSE营销活动的日志名称。</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 上次销售参与</td> 
   <td colspan="1">上次从销售部传入的参与。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE — 选择退出</td> 
   <td colspan="1">选择退出字段。</td> 
  </tr> 
 </tbody> 
</table>

## 按钮 {#buttons}

| **按钮名称** | **描述** |
|---|---|
| 发送MSE电子邮件 | 从Salesforce发送销售电子邮件。 |
| 添加到MSE营销活动 | 从Salesforce添加到MSE促销活动。 |
| 推送到MSE | 将联系人从Salesforce推送到MSE。 |
| 使用MSE调用 | 从Salesforce发出销售电话。 |

## 批量操作按钮 {#bulk-action-buttons}

| **按钮名称** | **描述** |
|---|---|
| 添加到MSE营销活动 | 从Salesforce添加到MSE促销活动。 |
| 推送到MSE | 将联系人从Salesforce推送到MSE。 |

## 用户指南 {#user-guides}

[Salesforce中的MSE自定义报表](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[Salesforce的MSE](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[Salesforce闪电的MSE](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
