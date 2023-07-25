---
unique-page-id: 5472615
description: 了解系统管理的字段 — Marketo文档 — 产品文档
title: 了解系统管理的字段
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# 了解系统管理的字段 {#understanding-system-managed-fields}

您可能会注意到 [人员详细信息页面](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} 包含由Marketo创建的一系列不可编辑的字段。 这些数据来自不同的来源，而且可以显示无数的值。

## 字段类型 {#field-types}

| **字段名称** | **条件** |
|---|---|
| 原始来源类型 | 首次发现人员或网站访客的位置（例如：列表导入、网页访问） |
| 原始来源信息 | 有关该位置的详细信息（例如：列表的名称、网页的URL） |
| 原始搜索引擎 | 如果适用，将人员引荐至原始条目源的搜索引擎 |
| 原始搜索短语 | 如果适用，则使用将人员引荐至原始条目源的搜索词 |
| 原始反向链接 | 托管原始登入源的URL |
| 注册源类型 | 活动首次成为人员的位置（例如：列表导入、网页访问） |
| 注册源信息 | 有关该位置的详细信息（例如：列表的名称、网页的URL） |
| 匿名 IP | 指示人员的IP地址 |
| 推断公司 | Marketo对个人公司的最佳猜测（基于IP） |
| 推断的城市 | Marketo对人员所在城市的最佳猜测（基于IP） |
| 推断的状态区域 | Marketo对人员所在州或地区的最佳猜测（基于IP） |
| 推断的邮政编码 | Marketo对人员邮政编码的最佳猜测（基于IP） |
| 推断的国家 | Marketo对人员所在国家/地区的最佳猜测（基于IP） |
| 推断的都市区 | Marketo对人员大都市区的最佳猜测（基于IP） |
| 推断的电话区号 | Marketo对人员区号的最佳猜测（基于IP） |

## 原始来源类型和登记来源类型的可能值 {#possible-values-for-original-and-registration-source-type}

以下是一些可能的值及其含义。

| **原始来源类型** | **条件** |
|---|---|
| Salesforce.com | 人员是从 [!DNL Webhook] 同步 |
| 网页访问量 | 从网页发现人员 |
| Web窗体填充 | 填写表单后发现人员 |
| 列表导入 | 从列表导入中发现人员 |
| 新人员 | 已将人员手动输入数据库 |
| Web链接单击 | 在单击链接后发现人员 |
| 销售电子邮件 | 通过以下方式向人员发送了电子邮件 [!DNL Sales Insight] 电子邮件加载项 |
| 人员 | 人员已从中同步 [!DNL Salesforce] 作为个人 |
| 联系人 | 人员已从中同步 [!DNL Webhook] 作为联系人 |
| [!DNL Munchkin] API | Marketo Engage发现人员 [!DNL Munchkin] API |
| 社交应用程序 | 社交小组件发现人员 |
| Web服务API | 通过Web服务API发现人员 |
| 活动合作伙伴 | 通过同步的网络研讨会服务发现人员 |
| 关联潜在客户 | 通过“关联潜在客户API”调用合并的人员 |

| **注册源类型** | **条件** |
|---|---|
| 列表导入 | 通过列表导入成为人员 |
| Salesforce.com | 通过 [!DNL Webhook] 同步 |
| Web窗体填充 | 在填写表单后成为了一个人 |
| 销售电子邮件 | 通过以下方式向人员发送了电子邮件 [!DNL Webhook] 电子邮件加载项 |
| Web服务API | 人员是通过SOAP/REST API创建的 |
| 新人员 | 已将人员手动输入数据库 |
| [!DNL Munchkin] API | 通过Marketo成为一个人 [!DNL Munchkin] API |
| 社交应用程序 | 通过社交小组件成为人 |
| 活动合作伙伴 | 通过链接的网络研讨会服务成为用户 |
