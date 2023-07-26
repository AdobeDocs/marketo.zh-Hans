---
unique-page-id: 4719314
description: 默认Salesforce字段映射 — Marketo文档 — 产品文档
title: 默认Salesforce字段映射
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 43%

---

# 默认Salesforce字段映射 {#default-salesforce-field-mapping}

当您最初将Marketo帐户与Salesforce同步时，Marketo会在您内置的Salesforce和Marketo字段之间自动建立这些关联。 Marketo还将同步您的Leads、Accounts、Opportunities和Contacts上的自定义字段。

## 潜在客户字段 {#lead-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 年收入 | 年收入 |
| 城市 | 城市 |
| 公司 | 公司名称 |
| 已转换日期 | SFDC 转化日期 |
| 国家 | 国家 |
| 创建日期 | SFDC创建日期 |
| 描述 | 人员备注 |
| 电子邮件 | 电子邮件地址 |
| 传真 | 传真号码 |
| 名字 | 名字 |
| 电子邮件选择退出 | 退订 |
| 行业 | 行业 |
| 已转换 | 已转换 SFDC |
| 已删除 | 已删除 SFDC |
| 姓氏 | 姓氏 |
| 潜在客户来源 | 源 |
| 潜在客户分数 | 得分 |
| 手机 | 手机号码 |
| 员工 | 员工数 |
| 电话 | 电话号码 |
| 邮政编码 | 邮政编码 |
| 评级 | 评级 |
| 称谓 | 称谓 |
| 省/市/自治区 | 州 |
| 状态 | 状态 |
| 街道 | 地址 |
| 标题 | 职务 |
| 网站 | 网站 |

## 联系人字段 {#contact-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 出生日期 | 出生日期 |
| 创建日期 | SFDC创建日期 |
| 联系人描述 | 人员备注 |
| 电子邮件 | 电子邮件地址 |
| 公司传真 | 传真号码 |
| 名字 | 名字 |
| 电子邮件选择退出 | 退订 |
| 已删除 | 已删除 SFDC |
| 姓氏 | 姓氏 |
| 潜在客户来源 | 源 |
| 潜在客户分数 | 得分 |
| 邮寄城市 | 城市 |
| MailingCountry | 国家 |
| MailingPostCode | 邮政编码 |
| MailingState | 州 |
| 邮寄街 | 地址 |
| 手机 | 手机号码 |
| 公司电话 | 电话号码 |
| 称谓 | 称谓 |
| 标题 | 职务 |

## 帐户字段 {#account-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 年收入 | 年收入 |
| 帐单寄送城市 | 帐单寄送城市 |
| 帐单寄送国家 | 帐单寄送国家 |
| 帐单邮编 | 帐单邮政编码 |
| 记帐省/市/自治区 | 帐单寄送州 |
| 帐单街道 | 帐单寄送地址 |
| 帐户说明 | 公司注释 |
| 行业 | 行业 |
| 已删除 | 已删除 SFDC |
| 帐户名称 | 公司名称 |
| 员工 | 员工数 |
| 帐户电话 | 主要电话 |
| SIC 代码 | SIC 代码 |
| 帐户站点 | 网站 |
| 帐户类型 | SFDC 类型 |
| 网站 | 网站 |

## Marketo中与Salesforce相关的系统字段（只读） {#salesforce-related-system-fields-in-marketo-read-only}

这些字段是在Marketo中创建的，但无法由客户调整。

| 字段 | 描述 |
|---|---|
| SFDC Id | 由18个字符组成的Salesforce Id |
| SFDC 类型 | 潜在客户或联系人。 如果为空，则商机在Marketo中仅作为人员存在 |
| SFDC创建日期 | 在SFDC中创建的日期(可以不同于在Marketo中创建的日期) |
| 已删除SFDC | 此人以前在SFDC工作，但已被删除，现在仅居住在Marketo |
