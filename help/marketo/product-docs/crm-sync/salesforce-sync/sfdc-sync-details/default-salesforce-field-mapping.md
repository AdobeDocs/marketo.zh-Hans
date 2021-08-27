---
unique-page-id: 4719314
description: 默认Salesforce字段映射 — Marketo文档 — 产品文档
title: 默认Salesforce字段映射
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 33%

---

# 默认Salesforce字段映射 {#default-salesforce-field-mapping}

最初，当您将Marketo帐户与Salesforce同步时，Marketo会自动在您内置的Salesforce和Marketo字段之间进行这些关联。 Marketo还将在您的潜在客户、帐户、机会和联系人上同步您的自定义字段。

## 潜在客户字段 {#lead-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 年营业额 | 年营业额 |
| 城市 | 城市 |
| 公司 | 公司名称 |
| 转换日期 | SFDC转换日期 |
| 国家 | 国家 |
| 创建日期 | SFDC创建日期 |
| 描述 | 人员说明 |
| 电子邮件 | 电子邮件地址 |
| 传真 | 传真号码 |
| 名字 | 名字 |
| 电子邮件选择退出 | 退订 |
| 行业 | 行业 |
| 已转换 | SFDC已转换 |
| 已删除 | 已删除SFDC |
| 姓氏 | 姓氏 |
| 潜在客户来源 | 源 |
| 潜在客户分数 | 得分 |
| 手机 | 手机号码 |
| 员工 | 员工数 |
| 电话 | 电话号码 |
| 邮政编码 | 邮政编码 |
| 评级 | 评级 |
| 称谓 | 称谓 |
| 州/省 | 州 |
| 状态 | 状态 |
| 街 | 地址 |
| 标题 | 职务 |
| 网站 | 网站 |

## 联系人字段 {#contact-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 出生日期 | 出生日期 |
| 创建日期 | SFDC创建日期 |
| 联系人描述 | 人员说明 |
| 电子邮件 | 电子邮件地址 |
| 商务传真 | 传真号码 |
| 名字 | 名字 |
| 电子邮件选择退出 | 退订 |
| 已删除 | 已删除SFDC |
| 姓氏 | 姓氏 |
| 潜在客户来源 | 源 |
| 潜在客户分数 | 得分 |
| MailingCity | 城市 |
| MailingCountry | 国家 |
| MailingPostalCode | 邮政编码 |
| MailingState | 州 |
| MailingStreet | 地址 |
| 手机 | 手机号码 |
| 商业电话 | 电话号码 |
| 称谓 | 称谓 |
| 标题 | 职务 |

## 帐户字段 {#account-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 年营业额 | 年营业额 |
| 帐单寄送城市 | 帐单寄送城市 |
| 帐单寄送国家 | 帐单寄送国家 |
| 帐单邮政编码 | 帐单邮政编码 |
| 账单州/省 | 帐单寄送州 |
| 比利街 | 帐单寄送地址 |
| 帐户描述 | 公司说明 |
| 行业 | 行业 |
| 已删除 | 已删除SFDC |
| 帐户名称 | 公司名称 |
| 员工 | 员工数 |
| 帐户电话 | 主要电话 |
| 标准产业分类(SIC)代码 | 标准产业分类(SIC)代码 |
| 帐户网站 | 现场 |
| 帐户类型 | SFDC类型 |
| 网站 | 网站 |

## Marketo中与Salesforce相关的系统字段（只读） {#salesforce-related-system-fields-in-marketo-read-only}

这些字段在Marketo中创建，但客户无法调整。

| 字段 | 描述 |
|---|---|
| SFDC Id | 18个字符的Salesforce Id |
| SFDC类型 | 潜在客户或联系人。 如果为空，则潜在客户仅作为人员存在在Marketo |
| SFDC创建日期 | 在SFDC中创建的日期(可以与在Marketo中创建的日期不同) |
| SFDC已删除 | 以前在SFDC工作的人员已被删除，现在只能在Marketo工作 |
