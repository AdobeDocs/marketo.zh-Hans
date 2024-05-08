---
description: 发行说明 — 2024年4月 — Marketo文档 — 产品文档
title: 发行说明 — 2024年4月
feature: Release Information
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 发行说明： 2024年4月 {#release-notes-apr-24}

在下方，您会找到2024年4月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

专门用于Adobe Dynamic Chat的发行说明 [可在此处找到](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，并将于以下日期开始发行 **2024年4月26日**，在接下来的几周内分阶段推出剩余的功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
     <tr> 
   <td><strong>交互式网络研讨会增强功能</strong>：现在，您可以让主机和演示者在事件投放后添加网络研讨会标题、重命名聊天室和手动同步参与数据。</td> 
   <td>已发货</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">创建交互式网络研讨会</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">手动同步</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>审核记录增强功能</strong>：现在可以在审核记录中捕获新类型的操作，这些操作涉及在字段管理中所做的更改、对用户和角色所做的更改以及从列表和智能列表导出的人员计数。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>新用户和角色权限</strong>：提供了新权限，为用户提供了更细粒度的Marketo Engage访问权限。 控制以前未控制的管理员部分（如新体验和预测受众），拆分权限以分别授予对资产审核记录和管理审核记录的访问权限，并利用资产和文件夹的新创建和移动权限来防止只读用户进行更改。 
   <p>虽然新权限将从4月26日起显示在您的Marketo Engage实例中，但目前它们处于被动状态，本季度晚些时候将可供访问。
   <li>访问Adobe Experience Manager</li>
   <li>访问Adobe组织映射</li>
   <li>访问管理员审核记录</li>
   <li>访问资产审核记录</li>
   <li>访问新体验</li>
   <li>访问预测受众</li>
   <li>创建报告</li>
   <li>创建列表</li>
   <li>导出营销活动活动</li>
   </td> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">角色权限描述</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **活动API更新**： 4月26日，我们将向基于Web和基于电子邮件的活动添加几个新属性，当您使用检索活动时，将返回这些属性 [MARKETO REST API](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} 端点可查看每个活动的属性详细信息。

**基于Web的活动**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">活动</th> 
   <th style="width:70%">新添加的属性</th>
   </tr>
  <tr> 
   <td>访问网页</td> 
   <td>浏览器、平台、设备</td>
  </tr>
   <tr> 
   <td>填写表单</td> 
   <td>浏览器、平台、设备</td>
  </tr>
  <tr> 
   <td>单击链接</td> 
   <td>浏览器、平台、设备</td>
  </tr>
 </tbody> 
</table>

**基于电子邮件的活动**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">活动</th> 
   <th style="width:70%">新添加的属性</th>
  </tr>
   <tr> 
   <td>发送电子邮件</td> 
   <td>浏览器、平台、设备、用户代理</td>
  </tr>
   </tr>
  <tr> 
   <td>电子邮件已送达</td> 
   <td>浏览器、平台、设备、用户代理</td>
  </tr>
   <tr> 
   <td>电子邮件已退回</td> 
   <td>浏览器、平台、设备、用户代理</td>
  </tr>
  <tr> 
   <td>取消订阅电子邮件</td> 
   <td>浏览器、平台、设备</td>
  </tr>
  <tr> 
   <td>打开电子邮件</td> 
   <td>浏览器</td>
  </tr>
   <tr> 
   <td>单击电子邮件</td> 
   <td>浏览器</td>
  </tr>
  <tr> 
   <td>电子邮件软退回</td> 
   <td>浏览器、平台、设备、用户代理</td>
  </tr>
 </tbody> 
</table>
