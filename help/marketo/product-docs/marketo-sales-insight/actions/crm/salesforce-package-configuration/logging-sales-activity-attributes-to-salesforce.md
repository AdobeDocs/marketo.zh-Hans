---
description: 将Sales Activity Attributes记录到Salesforce - Marketo Docs — 产品文档
title: 将销售活动属性记录到Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 5%

---

# 将销售活动属性记录到Salesforce {#logging-sales-activity-attributes-to-salesforce}

Salesforce管理员可以手动将自定义活动字段添加到Salesforce。

1. 在您的Salesforce帐户中，单击 **设置**.

1. 在快速搜索字段中搜索“活动自定义字段”，然后单击它。

1. 单击 **新**.

1. 根据下表选择与要添加字段对应的数据类型，然后单击 **下一个**.

1. 输入与要添加字段对应的字段名称和标签。

下表中各列的说明：

* **字段标签**：UI中显示的字段名称（可以自定义此名称以提高团队的可读性）
* **字段名称**：字段的技术名称（确保您输入的字段名称与下表中的字段名称匹配）
* **API名称**：API字段的技术名称（确保您输入的API名称与下表中的API名称匹配）
* **数据类型**：字段类型
* **大小**：文本字段的大小

<table>
 <tr>
  <th>字段标签</th>
  <th>字段名称</th>
  <th>API名称</th>
  <th>数据类型</th>
  <th>大小</th>
 </tr>
  <tr>
  <td>调用结果</td>
  <td>mktosales_call_output</td>
  <td>mktosales_call_output__c</td>
  <td>文本</td>
  <td>50</td>
 </tr>
 <tr>
  <td>致电原因</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>文本</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Marketo销售呼叫本地存在ID</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>文本</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo销售电话记录URL</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo促销活动</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>文本</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo促销活动当前步骤</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>文本</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo促销活动URL</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>已查看Marketo销售电子邮件附件</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
 <tr>
  <td>已单击Marketo销售电子邮件</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件已回复</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件状态</td>
  <td>mse_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>文本</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件模板</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>文本</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件模板URL</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件URL</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>已查看Marketo销售电子邮件</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
</table>
