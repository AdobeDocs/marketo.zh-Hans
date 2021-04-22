---
unique-page-id: 5472615
description: 了解系统管理字段 — Marketo文档 — 产品文档
title: 了解系统管理字段
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# 了解系统管理字段{#understanding-system-managed-fields}

您可能注意到，[人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)包含由Marketo创建的一系列不可编辑的字段。 这些数据来自不同的来源，有无数的价值可以显示。

## 字段类型{#field-types}

| **字段名称** | **定义** |
|---|---|
| 原始源类型 | 首次发现个人或网站访客的位置(示例：列表导入、网页访问) |
| 原始源信息 | 有关该位置的具体信息(示例：列表的名称，网页的URL) |
| 原始搜索引擎 | 如果适用，将人员引荐到原始输入源的搜索引擎 |
| 原始搜索短语 | 如果适用，则使用将人员引荐到原始输入源的搜索词 |
| 原始推荐人 | 托管原始条目源的URL |
| 注册源类型 | 活动首先成为人的位置(示例：列表导入、网页访问) |
| 注册源信息 | 有关该位置的具体信息(示例：列表的名称，网页的URL) |
| 匿名IP | 指示个人的IP地址 |
| 推断公司 | Marketo对个人公司的最佳猜测（基于IP） |
| 推断城市 | Marketo对个人城市的最佳猜测 |
| 推断的州 | Marketo对个人所在州或地区的最佳猜测（基于IP） |
| 推断的邮政编码 | Marketo对个人邮政编码的最佳猜测（基于IP） |
| 推断国家 | Marketo对个人国家/地区的最佳猜测（基于IP） |
| 推断的都市区 | Marketo对该人口大都区的最佳猜测（基于IP） |
| 推断出的电话区号 | Marketo对个人区号的最佳猜测（基于IP） |

## 原始和注册源类型{#possible-values-for-original-and-registration-source-type}的可能值

以下是一些可能的价值及其含义。

| **原始源类型** | **定义** |
|---|---|
| Salesforce.com | 从Salesforce同步中发现Person |
| 网页访问 | 在网页中发现了此人 |
| Web表单过滤 | 在填写表单后 |
| 列表导入 | 从列表导入中发现 |
| 新人 | 人员已手动输入数据库 |
| Web链接单击 | 在单击链接后发现人员 |
| 销售电子邮件 | Person已通过Sales Insight Email Add-In发送电子邮件 |
| 人 | Person已以个人身份从Salesforce同步 |
| 联系 | 已从Salesforce以联系人身份同步 |
| 蒙奇金API | Person是由Marketo的Munchkin API |
| 社交应用程序 | Person被一个社交小组件发现 |
| Web服务API | Person被Web服务API发现 |
| 事件合作伙伴 | 通过同步的网络研讨会服务发现此人 |
| 关联潜在客户 | 通过Associate Lead API调用合并的人 |

| **注册源类型** | **定义** |
|---|---|
| 列表导入 | 通过列表导入成为人 |
| Salesforce.com | 通过Salesforce同步成为人 |
| Web表单过滤 | 填好表单后成为人 |
| 销售电子邮件 | Person已通过Sales Insight Email Add-In发送电子邮件 |
| Web服务API | 人是通过SOAP/REST API创建的 |
| 新人 | 人员已手动输入数据库 |
| 蒙奇金API | 通过Marketo的Munchkin API成为 |
| 社交应用程序 | 通过社交构件成为人 |
| 事件合作伙伴 | 通过链接的网络研讨会服务成为人 |
