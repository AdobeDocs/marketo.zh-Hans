---
description: AWS迁移 — Marketo Engage文档 — 产品文档
title: AWS迁移
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 9c2784f06be42e5b65cd338a18b0d37a8fa48d9a
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 2%

---

# AWS迁移 {#aws-migration}

在接下来的几个月中，所有Marketo Engage订阅都将从专用数据中心迁移到AWS公共云，以提高可靠性、可扩展性和速度。

您将在迁移前约30天收到电子邮件以及应用程序内通知。 使用本指南进行准备。

## 建议的操作

在迁移期间，所有Marketo Engage服务将不可用。 我们建议您采取以下步骤来减轻对您的业务产生的任何影响。

* **避免创建或更新潜在客户/人员**，或避免运行修改人员记录的进程。

* **不触发后续流程**，因为计划的营销活动将暂停。

* **暂时禁用向Marketo Engage发送数据或从中接收数据的任何集成**。

* **避免运行**&#x200B;数据导入或导出或任何主要的潜在客户/人员生成营销活动。

* **审核并更新IP**&#x200B;登录、API访问、电子邮件发送、Web跟踪和集成。

* **添加新IP地址**&#x200B;并保留您当前的IP不变。 通过下面[&#128279;](#ip-addresses)的表查看要添加的IP地址。

## 预期的服务影响

您无需对以下影响执行任何操作。

* **CRM集成和LaunchPoint服务**&#x200B;将被禁用，但以后应自动恢复。
* **登陆页面、表单和数据收集**&#x200B;将不可用，并且将改为显示维护消息。

## 识别您的数据中心/面板 {#identify}

在查看以下表格之前，[了解如何识别](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify)您的订阅所在的数据中心和面板/服务器。

## 计划 {#schedule}

新的日期和数据中心/面板信息会定期添加，因此请务必返回此处查看详细信息。

<table>
 <tbody>
  <tr>
   <th style="width:50%">日期</th>
   <th style="width:20%">数据中心/面板</th>
   <th style="width:30%">时间</th>
  </tr>
  <tr>
   <td>2026年7月8日</td>
   <td>AB69<br>
   AB64</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
  </tr>
  <tr>
   <td>2026年7月9日</td>
   <td>AB70<br>
   AB43</td>
   <td>下午5点（太平洋夏令时间）<br>
   下午6点（太平洋夏令时间）</td>
  </tr>
  <tr>
   <td>2026年7月11日</td>
   <td>AB46</td>
   <td>上午10:00（太平洋夏令时间）</td>
  </tr>
  <tr>
   <td>2026年7月13日</td>
   <td>NLD101</td>
   <td>上午10:00（太平洋夏令时间）</td>
  </tr>
  <tr>
   <td>2026年7月15日</td>
   <td>NLD102<br>
   NLD104</td>
   <td>上午10:00（太平洋夏令时间）<br>
   上午11:00（太平洋夏令时间）</td>
  </tr>
  <tr>
   <td>2026年7月17日</td>
   <td>NLD103<br>
   NLD105</td>
   <td>上午10:00（太平洋夏令时间）<br>
   上午11:00（太平洋夏令时间）</td>
  </tr>
  &lt;/body>
</table>

## 要添加的IP地址 {#ip-addresses}

根据您的数据中心，与您的IT部门合作，添加各自的IP地址。

<table>
<tbody>
<tr>
  <th style="width:25%">数据中心</th>
  <th style="width:75%">IP地址</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
&lt;/body>
</table>

## 更新和支持

有关最新更新，请将此页加入书签。 如果您有任何问题，请通过Admin Console或[Experience League](https://experienceleague.adobe.com/en/support){target="_blank"}中的支持门户联系Adobe支持部门。
