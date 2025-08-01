---
description: 为新的Marketo Engage实例设置Database部分。
title: 新实例最佳实践 — 数据库核对清单
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 2%

---

# 新实例最佳实践：数据库核对清单 {#new-instance-best-practices-database-checklist}

在“数据库”部分中，您可以找到实例中人员的关键属性。 了解更多有关在数据库中的不同列表和分段中导航以及管理人员记录所需的步骤。

请记住[下载核对清单](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)并跟踪您的进度。

## 系统智能列表 {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>所有人员</td>
    <td><li>确定与您的CRM实施1:1同步或应用过滤器以限制从系统移动到系统的人员和时间。</li>
    <li>查看<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=zh-Hans" target="_blank">Marketo Engage数据库</a>中的人员和可营销人员总数。</li></td>
  </tr>
  <tr>
    <td>阻止列表</td>
    <td><li>定义阻止列表标准。 考虑将竞争对手的域添加到您的<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=zh-Hans" target="_blank">阻止列表</a>，以防止他们接收您的任何电子邮件。</li></td>
  </tr>
  <tr>
    <td>营销暂停</td>
    <td><li>定义<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">营销暂停</a>条件。</li></td>
  </tr>
  <tr>
    <td>退回的电子邮件地址 </td>
    <td><li>为退回的电子邮件地址定义条件。</li>
    <li>查看“电子邮件无效”类别中的人员并确定其电子邮件是否需要<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=zh-Hans" target="_blank">手动重置</a>。</li></td>
  </tr>
  <tr>
    <td>可能的重复项</td>
    <td><li>查看可能重复项列表中的人员。</li>
    <li>定义复写管理策略以确定是否要手动<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=zh-Hans" target="_blank">合并人员</a>。</li>
    <li>如果您拥有CRM集成，请定义一个流程和帐户，以处理CRM中合并潜在客户的<a href="https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">效果</a>。</li></td>
  </tr>
  <tr>
    <td>无客户获取计划</td>
    <td><li>在您的项目模板中建立营销活动，以设置客户获取项目，尤其是使用全局表单时。</li></td>
  </tr>
  <tr>
    <td>已取消订阅的人员</td>
    <td><li>查看<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=zh-Hans" target="_blank">已取消订阅的人员</a>的标准。</li></td>
  </tr>
</tbody>
</table>

## 组智能列表 {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">面积</th>
    <th style="width:80%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>组智能列表</td>
    <td><li>请注意创建组智能列表，这样就不会有重复的列表。</li>
    <li>跟踪数据库中的主列表。</li></td>
  </tr>
</tbody>
</table>

## 区段 {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">面积</th>
    <th style="width:79%">操作项</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>区段</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=zh-Hans" target="_blank">根据您的业务需求创建分段</a>。 每个订购限制为20个区段，每个区段内有100个区段。</li></td>
  </tr>
</tbody>
</table>
