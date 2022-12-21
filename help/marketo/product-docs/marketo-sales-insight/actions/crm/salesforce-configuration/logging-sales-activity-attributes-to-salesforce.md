---
description: 将销售活动属性记录到Salesforce - Marketo文档 — 产品文档
title: 将销售活动属性记录到Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 9f3b91e7b0626b2a229f4a98fb734e926a141ec0
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 5%

---

# 将销售活动属性记录到Salesforce {#logging-sales-activity-attributes-to-salesforce}

Salesforce管理员可以手动将自定义活动字段添加到Salesforce。

1. 在您的Salesforce帐户中，单击 **设置**.

1. 在快速搜索字段中搜索“活动自定义字段”，然后单击该字段。

1. 单击 **新建**.

1. 根据下表选择要添加的字段对应的数据类型，然后单击 **下一个**.

1. 输入与要添加的字段对应的字段名称和标签。

下表中每列的描述：

* **字段标签**:UI中显示的字段名称（您的团队可以自定义此名称，以提高可读性）
* **字段名称**:字段的技术名称（确保您输入的字段名称与下表中的字段名称匹配）
* **API名称**:API字段的技术名称（确保您输入的API名称与下表中的API名称相匹配）
* **数据类型**:字段类型
* **大小**:文本字段的大小

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
  <td>mktosales_call_outde</td>
  <td>mktosales_call_outde__c</td>
  <td>文本</td>
  <td>50</td>
 </tr>
 <tr>
  <td>呼叫原因</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>文本</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Marketo销售电话本地存在ID</td>
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
  <td>Marketo Sales Campaign</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>文本</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo销售活动当前步骤</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>文本</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Marketo销售活动URL</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo已查看的销售电子邮件附件</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件已点击</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件已回复</td>
  <td>MSE_Reploded</td>
  <td>MSE_Reploded__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
 <tr>
  <td>Marketo销售电子邮件状态</td>
  <td>MSE_Email_Status</td>
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
  <td>Marketo已查看的销售电子邮件</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed__c</td>
  <td>复选框</td>
  <td></td>
 </tr>
</table>
