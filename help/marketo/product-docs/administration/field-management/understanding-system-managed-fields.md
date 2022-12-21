---
unique-page-id: 5472615
description: 了解系统管理的字段 — Marketo文档 — 产品文档
title: 了解系统管理的字段
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 5%

---

# 了解系统管理的字段 {#understanding-system-managed-fields}

您可能注意到 [人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) 具有Marketo创建的一系列不可编辑的字段。 这些数据来自各种来源，可以显示无数值。

## 字段类型 {#field-types}

| **字段名称** | **条件** |
|---|---|
| 原始源类型 | 首次发现人员或网站访客的位置(示例：列表导入，网页访问) |
| 原始源信息 | 有关该位置的具体说明(示例：列表名称，网页的URL) |
| 原始搜索引擎 | 如果适用，将人员引荐至原始输入源的搜索引擎 |
| 原始搜索短语 | 如果适用，则将人员引荐至原始输入来源的搜索词 |
| 原始反向链接 | 托管原始登入源的URL |
| 注册来源类型 | 活动首次成为人员的位置(示例：列表导入，网页访问) |
| 注册源信息 | 有关该位置的具体说明(示例：列表名称，网页的URL) |
| 匿名 IP | 指示人员的IP地址 |
| 推断公司 | Marketo对该人员公司的最佳猜测（基于IP） |
| 推断的城市 | Marketo对人员城市的最佳猜测（基于IP） |
| 推断的状态区域 | Marketo对人员所在州或地区的最佳猜测（基于IP） |
| 推断的邮政编码 | Marketo对人员邮政编码的最佳猜测（基于IP） |
| 推断的国家 | Marketo对个人国家/地区的最佳猜测（基于IP） |
| 推断的都市区 | Marketo人口大都市区的最佳猜测（基于IP） |
| 推断的电话区号 | Marketo人员区号的最佳猜测（基于IP） |

## 原始和注册来源类型的可能值 {#possible-values-for-original-and-registration-source-type}

以下是一些可能的值及其含义。

| **原始源类型** | **条件** |
|---|---|
| Salesforce.com | 从Salesforce同步中发现了人员 |
| 网页访问量 | 从网页中发现了人 |
| Web窗体过滤器 | 填完表格后发现人 |
| 列表导入 | 从列表导入中发现人员 |
| 新人 | 人员已手动输入数据库 |
| Web链接点击 | 单击链接后发现人员 |
| 销售电子邮件 | Person是通过Sales Insight Email Add-In发送的电子邮件 |
| 人员 | 人员是作为人员从Salesforce同步的 |
| 联系人 | 人员是作为联系人从Salesforce同步的 |
| 蒙奇金API | Marketo的Munchkin API发现了该人 |
| 社交应用程序 | 社交小组件发现了人 |
| Web服务API | Web服务API发现了人员 |
| 活动合作伙伴 | 已同步的网络研讨会服务会发现人员 |
| 关联潜在客户 | 通过关联潜在客户API调用合并的人员 |

| **注册来源类型** | **条件** |
|---|---|
| 列表导入 | 通过列表导入成为人员 |
| Salesforce.com | 通过Salesforce同步成为人 |
| Web窗体过滤器 | 填完表格后成了人 |
| 销售电子邮件 | Person是通过Sales Insight Email Add-In发送的电子邮件 |
| Web服务API | 人员是通过SOAP/REST API创建的 |
| 新人 | 人员已手动输入数据库 |
| 蒙奇金API | 通过Marketo的Munchkin API成为人物 |
| 社交应用程序 | 通过社交小组件成为人 |
| 活动合作伙伴 | 通过链接的网络研讨会服务成为人员 |
