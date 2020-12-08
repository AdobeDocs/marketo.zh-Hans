---
unique-page-id: 4719314
description: 默认Salesforce字段映射- Marketo文档——产品文档
title: 默认Salesforce字段映射
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 默认Salesforce字段映射 {#default-salesforce-field-mapping}

当您最初将Marketo帐户与Salesforce同步时，Marketo会自动在您的内置Salesforce和Marketo字段之间建立这些关联。 Marketo还将同步您的Lead、Accounts、Opportunity和Contacts上的自定义字段。

## 潜在客户字段 {#lead-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 年收入 | 年收入 |
| 城市 | 城市 |
| 公司 | 公司名称 |
| 转换日期 | SFDC转换日期 |
| 国家／地区 | 国家／地区 |
| 创建日期 | SFDC创建日期 |
| 说明 | 人员说明 |
| 电子邮件 | 电子邮件地址 |
| 传真 | 传真号码 |
| 名字 | 名字 |
| 电子邮件选择退出 | 取消订阅 |
| 行业 | 行业 |
| 已转换 | SFDC已转换 |
| 已删除 | SFDC已删除 |
| 姓氏 | 姓氏 |
| 潜在客户来源 | 源 |
| 潜在客户得分 | 得分 |
| 手机 | 手机号码 |
| 员工 | 员工人数 |
| 电话 | 电话号码 |
| 邮政编码 | 邮政编码 |
| 评级 | 评级 |
| 问候 | 问候 |
| 州／省 | 州 |
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
| 电子邮件选择退出 | 取消订阅 |
| 已删除 | SFDC已删除 |
| 姓氏 | 姓氏 |
| 潜在客户来源 | 源 |
| 潜在客户得分 | 得分 |
| MailingCity | 城市 |
| MailingCountry | 国家／地区 |
| MailingPostalCode | 邮政编码 |
| MailingState | 州 |
| MaingStreet | 地址 |
| 手机 | 手机号码 |
| 商务电话 | 电话号码 |
| 问候 | 问候 |
| 标题 | 职务 |

## 帐户字段 {#account-fields}

| SFDC字段 | Marketo字段 |
|---|---|
| 年收入 | 年收入 |
| 计费城市 | 计费城市 |
| 帐单国 | 帐单国 |
| 帐单邮政编码 | 帐单邮政编码 |
| 结算州／省 | 帐单状态 |
| 帐单街 | 帐单地址 |
| 帐户说明 | 公司说明 |
| 行业 | 行业 |
| 已删除 | SFDC已删除 |
| 帐户名称 | 公司名称 |
| 员工 | 员工人数 |
| 帐户电话 | 主电话 |
| SIC代码 | SIC代码 |
| 帐户站点 | 站点 |
| 帐户类型 | SFDC类型 |
| 网站 | 网站 |

## Marketo中的Salesforce相关系统字段（只读） {#salesforce-related-system-fields-in-marketo-read-only}

这些字段在Marketo中创建，但客户无法调整。

| 字段 | 说明 |
|---|---|
| SFDC ID | 18个字符的Salesforce Id |
| SFDC类型 | 潜在客户或联系人。 如果为空，则潜在客户仅作为Marketo中的人员存在 |
| SFDC创建日期 | 在SFDC中创建的日期（可以不同于在Marketo中创建的日期） |
| SFDC已删除 | 人员过去在SFDC中，但已被删除，现在仅在Marketo中居住 |
