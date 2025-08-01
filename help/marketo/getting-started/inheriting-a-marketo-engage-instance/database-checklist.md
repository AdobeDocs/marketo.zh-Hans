---
description: 继承实例数据库核对清单 — Marketo文档 — 产品文档
title: 继承实例数据库核对清单
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 2%

---

# 继承的实例：数据库核对清单 {#inherited-instance-database-checklist}

了解您的订阅中的总人数、可营销人员和主要人员获取来源。 请记住[下载核对清单](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx)并跟踪您的进度。

## 系统智能列表 {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>所有人员</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">数据库</a>中有多少人？</li>
<li>如果数据库已接近满，您的公司策略是否建议扩大数据库大小或清除历史数据？</li>
<li>您的总体数据库是否至少有85%是适销的？
<br/>     列入阻止列表如果您未达到此阈值，请仔细查看其他系统智能列表（、营销暂停、重复、取消订阅）。</li></td>
  </tr>
  <tr>
   <td>已取消订阅的人员</td>
   <td><li>您对<a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">已取消订阅的用户</a>的标准是什么？ 是否有太多未订阅的人员？</li>
<li>您的取消订阅方法是否符合您的数据隐私要求？</li>
<li>您的取消订阅首选项是否为最新？ 记录在数据库中作为不可销售记录保留多长时间？</li></td>
  </tr>
  <tr>
   <td>营销暂停</td>
   <td><li>您的<a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">营销暂停</a>条件是什么？ 营销被暂停的人数是否太多？</li>
<li>记录保留营销暂停状态多长时间？</li>
<p>“营销已暂停”用例示例：人员记录积极参与您想要为其抑制营销沟通的后期商机的销售。</td>
  </tr>
   <tr>
   <td>阻止列表</td>
   <td><li>您的<a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">列入阻止列表记录</a>标准是什么？ 被列入阻止列表的人是否太多？</li></td>
  </tr>
  <tr>
   <td>退回的电子邮件地址</td>
   <td><li>您的数据库中是否有许多<a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">人退回</a>？
   <br/>     如果是这样的话，请考虑调查一下原因。</li></td></li></td>
  </tr>
  <tr>
   <td>可能的重复项</td>
   <td><li>有多少<a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">条可能重复的记录</a>？
   <br/>     请考虑删除或合并它们。</li></td>
  </tr>
   <tr>
   <td>无客户获取计划</td>
   <td><li>有多少人没有<a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">客户获取计划</a>？
   <br/>     如果有很多，请考虑调查原因。</li></td>
  </tr>
 </tbody>
</table>

## 智能列表 {#smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>智能列表</td>
   <td><li>有多少个<a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">智能列表</a>？ 在本例中如何使用它们？</li>
   <p><img src="assets/note-icon.png" alt="注释图标"> 注：在“数据库”部分中，组智能列表是用户生成的，系统智能列表是Marketo Engage创建的默认列表。
<li>列表是否以具有凝聚力的文件夹结构组织？
<br/>     如果您有孤立列表，请考虑组织您的树，以便轻松找到资产。</li>
<p><img src="assets/tip-icon.png" alt="提示图标">提示： <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">存档</a>不再需要的智能列表将有助于组织和性能。</td>
  </tr>
 </tbody>
</table>

## 静态列表 {#static-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>静态列表</td>
   <td><li>有多少个<a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">静态列表</a>？ 在本例中如何使用它们？</li>
   <p><img src="assets/note-icon.png" alt="注释图标"> 注：在“数据库”部分中，组列表是静态列表。</td>
  </tr>
 </tbody>
</table>

## 分段 {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">面积</th>
   <th>审核焦点</th>
  </tr>
  <tr>
   <td>分段</td>
   <td><li>存在哪些<a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">分段</a>？ 它们是如何被使用的？</li>
<li><a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">默认区段</a>是否包含太多人员？</li>
<li>是否有针对可营销受众的分段？
<br/>     如果不能，请考虑创建一个。</li></td>
  </tr>
 </tbody>
</table>
