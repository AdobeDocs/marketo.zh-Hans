---
unique-page-id: 5472615
description: 了解系统管理字段- Marketo Docs —— 产品文档
title: 了解系统管理字段
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# 了解系统管理字段{#understanding-system-managed-fields}

您可能已经注意到[人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)包含由Marketo创建的一系列不可编辑字段。 这些数据来自不同的来源，有无数的价值可以展示。

## 字段类型{#field-types}

| **字段名称** | **定义** |
|---|---|
| 原始源类型 | 首次发现个人或网站访客的位置(示例：列表导入，网页访问) |
| 原始源信息 | 有关该位置的特定信息(示例：列表的名称、网页的URL) |
| 原始搜索引擎 | 如果适用，将人员引用到原始输入源的搜索引擎 |
| 原始搜索短语 | 如果适用，则使用将人员引用到原始输入源的搜索词 |
| 原始推荐人 | 托管原始输入源的URL |
| 注册源类型 | 活动首先变成人员的位置(示例：列表导入，网页访问) |
| 注册源信息 | 有关该位置的特定信息(示例：列表的名称、网页的URL) |
| 匿名IP | 指示人员的IP地址 |
| 推断公司 | Marketo对个人公司的最佳猜测（基于IP） |
| 推断城市 | Marketo对个人城市的最佳猜测 |
| 推断的州区 | Marketo对个人所在州或地区的最佳猜测（基于IP） |
| 推断的邮政编码 | Marketo对个人邮政编码的最佳猜测（基于IP） |
| 推断国家 | Marketo对个人国家的最佳猜测（基于IP） |
| 推断的都市区 | Marketo对人口大都市区的最佳猜测（基于IP） |
| 推断电话区号 | Marketo对个人区号的最佳猜测（基于IP） |

## 原始和注册源类型{#possible-values-for-original-and-registration-source-type}的可能值

以下是一些可能的价值及其含义。

| **原始源类型** | **定义** |
|---|---|
| Salesforce.com | 在Salesforce同步中发现人员 |
| 网页访问 | 从网页中发现人物 |
| Web表单过滤 | 填写表单后发现人 |
| 列表导入 | 从列表导入中发现人员 |
| 新人 | 人员已手动输入数据库 |
| Web链接单击 | 在单击链接后发现人员 |
| 销售电子邮件 | Person beas sels Insight Email Add-In发送电子邮件 |
| 人物 | Person was synced over from Salesforce as person |
| 联系 | 人员从Salesforce同步为联系人 |
| 蒙奇金API | Person is be soved by Marketo&#39;s Munchkin API |
| 社交应用程序 | 人被一个社交小部件发现 |
| Web服务API | Person被Web服务API发现 |
| 事件合作伙伴 | 通过同步的网络研讨会服务发现人员 |
| 关联潜在客户 | 通过Associate Lead API调用合并的人员 |

| **注册源类型** | **定义** |
|---|---|
| 列表导入 | 通过列表进口成为人 |
| Salesforce.com | 通过Salesforce同步成为人 |
| Web表单过滤 | 填写表格后成为人 |
| 销售电子邮件 | Person beas sels Insight Email Add-In发送电子邮件 |
| Web服务API | 人是通过SOAP/REST API创建的 |
| 新人 | 人员已手动输入数据库 |
| 蒙奇金API | 通过Marketo的Munchkin API成为 |
| 社交应用程序 | 通过社交构件成为人 |
| 事件合作伙伴 | 通过链接的网络研讨会服务成为人物 |
