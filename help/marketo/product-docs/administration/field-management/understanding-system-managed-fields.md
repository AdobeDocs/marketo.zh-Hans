---
unique-page-id: 5472615
description: 了解系统管理的字段 — Marketo文档 — 产品文档
title: 了解系统管理字段
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 11%

---

# 了解系统管理字段 {#understanding-system-managed-fields}

您可能已经注意到[人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}包含由Marketo创建的一系列不可编辑的字段。 这些数据来自不同的来源，而且有无数值可以显示。

## 字段类型 {#field-types}

<table><thead>
  <tr>
    <th>字段名称</th>
    <th>定义</th>
  </tr></thead>
<tbody>
  <tr>
    <td>原始来源类型</td>
    <td>首次发现人员或网站访客的位置（例如：列表导入、网页访问）</td>
  </tr>
  <tr>
    <td>原始来源信息</td>
    <td>有关该位置的详细信息（示例：列表的名称、网页的URL）</td>
  </tr>
  <tr>
    <td>原始搜索引擎</td>
    <td>如果适用，将人员引荐至原始条目来源的搜索引擎</td>
  </tr>
  <tr>
    <td>原始搜索短语</td>
    <td>如果适用，使用的搜索词将人员引荐至原始条目源</td>
  </tr>
  <tr>
    <td>原始反向链接</td>
    <td>托管原始登入源的URL</td>
  </tr>
  <tr>
    <td>注册Source类型</td>
    <td>活动首次成为人员的位置（例如：列表导入、网页访问）</td>
  </tr>
  <tr>
    <td>注册Source信息</td>
    <td>有关该位置的详细信息（示例：列表的名称、网页的URL）</td>
  </tr>
  <tr>
    <td>匿名 IP</td>
    <td>指示人员的IP地址</td>
  </tr>
  <tr>
    <td>推断公司</td>
    <td>Marketo对个人公司的最佳猜测（基于IP）</td>
  </tr>
  <tr>
    <td>推断的城市</td>
    <td>Marketo对个人所在城市的最佳猜测（基于IP）</td>
  </tr>
  <tr>
    <td>推断的状态区域</td>
    <td>Marketo对个人所在州或地区的最佳猜测（基于IP）</td>
  </tr>
  <tr>
    <td>推断的邮政编码</td>
    <td>Marketo对人员邮政编码的最佳猜测（基于IP）</td>
  </tr>
  <tr>
    <td>推断的国家</td>
    <td>Marketo对个人所在国家/地区的最佳猜测（基于IP）</td>
  </tr>
  <tr>
    <td>推断的都市区</td>
    <td>Marketo对人员大都市区的最佳猜测（基于IP）</td>
  </tr>
  <tr>
    <td>推断的电话区号</td>
    <td>Marketo对人员区号的最佳推测（基于IP）</td>
  </tr>
</tbody></table>

## 原始和注册Source类型的可能值 {#possible-values-for-original-and-registration-source-type}

以下是一些可能的值及其含义。

<table><thead>
  <tr>
    <th>原始来源类型</th>
    <th>定义</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>从Salesforce同步发现人员</td>
  </tr>
  <tr>
    <td>网页访问量</td>
    <td>从网页发现人员</td>
  </tr>
  <tr>
    <td>Web窗体填充</td>
    <td>填写表单后发现人员</td>
  </tr>
  <tr>
    <td>列表导入</td>
    <td>从列表导入中发现人员</td>
  </tr>
  <tr>
    <td>新人员</td>
    <td>已将人员手动输入数据库</td>
  </tr>
  <tr>
    <td>Web链接点击</td>
    <td>单击链接后发现人员</td>
  </tr>
  <tr>
    <td>销售电子邮件</td>
    <td>通过Sales Insight电子邮件加载项向人员发送了一封电子邮件</td>
  </tr>
  <tr>
    <td>人员</td>
    <td>人员已作为人员从Salesforce同步</td>
  </tr>
  <tr>
    <td>联系人</td>
    <td>人员已作为联系人从Webhook同步</td>
  </tr>
  <tr>
    <td>MUNCHKIN API</td>
    <td>通过Marketo Engage Munchkin API发现人员</td>
  </tr>
  <tr>
    <td>社交应用程序</td>
    <td>人员已由社交小组件发现</td>
  </tr>
  <tr>
    <td>Web服务API</td>
    <td>通过Web服务API发现人员</td>
  </tr>
  <tr>
    <td>活动合作伙伴</td>
    <td>通过同步的网络研讨会服务发现人员</td>
  </tr>
  <tr>
    <td>关联潜在客户</td>
    <td>通过关联潜在客户API调用合并的人员</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>注册Source类型</th>
    <th>定义</th>
  </tr></thead>
<tbody>
  <tr>
    <td>列表导入</td>
    <td>通过列表导入成为人员</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>通过Salesforce sync成为人员</td>
  </tr>
  <tr>
    <td>Web窗体填充</td>
    <td>在填写表单后成为了一个人</td>
  </tr>
  <tr>
    <td>销售电子邮件</td>
    <td>通过Sales Insight电子邮件加载项向人员发送了一封电子邮件</td>
  </tr>
  <tr>
    <td>Web服务API</td>
    <td>人员是通过SOAP/REST API创建的</td>
  </tr>
  <tr>
    <td>新人员</td>
    <td>已将人员手动输入数据库</td>
  </tr>
  <tr>
    <td>MUNCHKIN API</td>
    <td>通过Marketo的Munchkin API成为用户</td>
  </tr>
  <tr>
    <td>社交应用程序</td>
    <td>通过社交小组件成为人</td>
  </tr>
  <tr>
    <td>活动合作伙伴</td>
    <td>通过链接的网络研讨会服务成为个人</td>
  </tr>
</tbody>
</table>
