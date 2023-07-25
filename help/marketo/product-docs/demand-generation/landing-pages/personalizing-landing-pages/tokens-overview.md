---
unique-page-id: 2950799
description: 令牌概述 — Marketo文档 — 产品文档
title: 令牌概述
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 令牌概述 {#tokens-overview}

令牌是一个变量，可用于Marketo智能营销活动流程步骤、电子邮件、登陆页面、代码片段和Web营销活动。

## 了解默认值 {#understanding-default-values}

当您使用令牌时，还需要提供默认值。 这是显示某人是否没有您引用的字段值的文本。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此示例中，电子邮件将显示“Greetings， (first name)”或“Greetings， earthling”（默认值）。

![](assets/two.png)

>[!CAUTION]
>
>使用Marketo的电子邮件编辑器时，令牌在预标头中无法正常工作。 要在预标头中使用令牌，它必须通过您在电子邮件模板中自己的HTML。

>[!NOTE]
>
>这份清单并非详尽无遗。 此外，还会为您在Marketo中拥有的每个自定义字段创建令牌。

## 人员令牌 {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* 如果您使用其显示名称，自定义人员字段也可正常工作，例如， `{{lead.Custom Field Name}}`

## 公司令牌 {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* 如果您使用自定义公司字段的显示名称，例如 `{{Company.Custom Field Name}}`

## 营销活动令牌 {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系统令牌 {#system-tokens}

>[!NOTE]
>
>要了解有关这些令牌的更多信息，请参阅 [系统令牌术语表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## 触发器令牌 {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>查找更多有关 [有趣时刻的令牌](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) 基于智能营销活动中使用的触发器。

## 项目令牌 {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## 我的令牌 {#my-tokens}

我的Token是在项目中定义的，并且以 `{{my.` 后跟您为令牌创建的名称。 详细了解 [程序中的我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## 成员令牌 {#member-token}

成员令牌用于插入来自集成服务合作伙伴的唯一值。 成员令牌的常见用途是网络研讨会出席者的唯一URL。 每个人都有一个访问网络研讨会的唯一URL，可使用插入 `{{member.webinar url}}` 令牌。 此 `{{member.webinar url}}` 令牌会自动解析服务提供商生成的人员的唯一确认URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>此 `{{member.webinar url}}` 仅当发送电子邮件的智能营销活动是事件程序的子资产时，才会填充令牌。
