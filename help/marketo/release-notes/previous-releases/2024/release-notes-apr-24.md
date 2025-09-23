---
description: 发行说明 — 2024年4月 — Marketo文档 — 产品文档
title: 发行说明 - 2024 年 4 月
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 21%

---

# 发行说明：2024 年 4 月 {#release-notes-apr-24}

在下方，您会找到2024年4月版本中包含的所有功能。 请检查您的 Adobe Marketo Engage 版本以确认功能可用性。

Adobe Dynamic Chat 的专用发行说明[可在此处查看](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}。

>[!AVAILABILITY]
>
>带有星标（![star](assets/yellow-star.png)）的功能为付费附加组件。请联系您的 Marketo Engage 代表了解更多信息。

## 标准发布周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2024年4月26日**&#x200B;开始发行，并在接下来的几周内分阶段推出剩余功能。 功能及发布时间可能会有变动。请查看每个功能旁的状态标记。

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">功能</th>
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
     <tr>
   <td><strong>交互式网络研讨会增强功能</strong>：您现在可以为主持人和演示者提供以下功能：添加网络研讨会标题、重命名聊天室，以及在事件交付后手动同步参与数据。</td>
   <td>已发布</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">创建交互式网络研讨会</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">手动同步</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>审核记录增强功能</strong>：
   现在，可以在审计跟踪中捕获新类型的操作，这些操作涉及在字段管理中所做的更改、对用户和角色所做的更改以及从列表和智能列表导出的人员计数。</td>
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>新用户和角色权限</strong>：有新权限可用，为用户提供了对Marketo Engage的更细粒度访问权限。 控制以前未控制的管理员部分（如新体验和预测受众），拆分权限以分别授予对资产审核记录和管理审核记录的访问权限，并利用资产和文件夹的新创建和移动权限来防止只读用户进行更改。
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
   <td>已发布</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">角色权限说明</a></td>
  </tr>
 </tbody>
</table>
<br/>

## 公告 {#announcements}

* **活动API更新**： 4月26日，我们将向使用[Marketo REST API](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}检索活动时返回的基于Web和基于电子邮件的活动添加几个新属性。 下面列出的活动现在包括“浏览器”、“平台”、“设备”和“用户代理”属性。 调用[获取活动类型](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"}端点以查看每个活动的属性详细信息。

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
   <td>点击电子邮件</td>
   <td>浏览器</td>
  </tr>
  <tr>
   <td>电子邮件软退回</td>
   <td>浏览器、平台、设备、用户代理</td>
  </tr>
 </tbody>
</table>
