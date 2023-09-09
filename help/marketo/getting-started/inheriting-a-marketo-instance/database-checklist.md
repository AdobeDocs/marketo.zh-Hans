---
description: 继承实例数据库核对清单 — Marketo文档 — 产品文档
title: 继承实例数据库核对清单
hide: true
hidefromtoc: true
source-git-commit: 74afe85b5d7b78cc4bce3e2ec89cb5c1a56d2f59
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# 继承的实例：数据库核对清单 {#inherited-instance-database-checklist}

了解您的订阅中的总人数、可营销人员和主要人员获取来源。

## 系统智能列表 {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th> 
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>所有人员</td> 
   <td><li>有多少人存在于 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">数据库</a>？</li>
<li>如果数据库已接近满，您的公司策略是否建议扩大数据库大小或清除历史数据？</li>
<li>您的总体数据库是否至少有85%是适销的？ 
<br/>     列入阻止列表如果您未达到此阈值，请仔细查看其他系统智能列表（、营销暂停、重复、取消订阅）。</li></td>
  </tr>
  <tr> 
   <td>已取消订阅的人员</td> 
   <td><li>您的标准是什么 <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">已取消订阅的人员</a>？ 是否有太多未订阅的人员？</li>
<li>您的取消订阅方法是否符合您的数据隐私要求？</li>
<li>您的取消订阅首选项是否为最新？ 记录在数据库中作为不可销售记录保留多长时间？</li></td>
  </tr>
  <tr> 
   <td>营销暂停</td> 
   <td><li>您的标准是什么 <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">营销已暂停</a>？ 营销被暂停的人数是否太多？</li>
<li>记录保留营销暂停状态多长时间？</li>
<p>“营销已暂停”用例示例：人员记录积极参与您想要为其抑制营销沟通的后期商机的销售。</td>
  </tr>
   <tr> 
   <td>阻止列表</td> 
   <td><li>您的标准是什么 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">列入阻止列表记录</a>？ 被列入阻止列表的人是否太多？</li></td>
  </tr>
  <tr> 
   <td>退回的电子邮件地址</td> 
   <td><li>你有很多 <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">退回的人员</a> 在数据库中？
   <br/>     如果是这样的话，请考虑调查一下原因。</li></td></li></td>
  </tr>
  <tr> 
   <td>可能的重复项</td> 
   <td><li>数量 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">可能重复的记录</a> 有吗？
   <br/>     请考虑删除或合并它们。</li></td>
  </tr>
   <tr> 
   <td>无客户获取计划</td> 
   <td><li>有多少人没有 <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">客户获取计划</a>？
   <br/>     如果有很多，请考虑调查原因。</li></td>
  </tr>
 </tbody> 
</table>

## 智能列表 {#smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th> 
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>智能列表</td> 
   <td><li>数量 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">智能列表</a> 有吗？ 在本例中如何使用它们？</li>
<li>列表是否以具有凝聚力的文件夹结构组织？ 
<br/>     如果您有孤立列表，请考虑组织您的树，以便轻松找到资产。</li>
<p><img src="assets/tip-icon.png" alt="提示图标">提示： <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">正在存档</a> 不再需要的智能列表将有助于组织和性能。</td>
  </tr>
 </tbody> 
</table>

## 静态列表 {#static-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th> 
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>静态列表</td> 
   <td><li>数量 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">静态列表</a> 有吗？ 在本例中如何使用它们？</li></td>
  </tr>
 </tbody> 
</table>

## 分段 {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">区域</th> 
   <th>审核焦点</th>
  </tr> 
  <tr> 
   <td>分段</td> 
   <td><li>哪个 <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">分段</a> 有吗？ 它们是如何被使用的？</li>
<li>有太多人在 <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">默认区段</a>？</li>
<li>是否有针对可营销受众的分段？ 
<br/>     如果不能，请考虑创建一个。</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[◄审核继承的实例：管理员](/help/marketo/getting-started/inheriting-a-marketo-instance/admin-section-checklist.md)

[审核继承的实例：营销活动►](/help/marketo/getting-started/inheriting-a-marketo-instance/marketing-activities-checklist.md)
