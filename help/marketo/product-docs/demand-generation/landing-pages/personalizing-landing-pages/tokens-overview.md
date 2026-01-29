---
unique-page-id: 2950799
description: 令牌概述 — Marketo 文档 — 产品文档
title: 令牌概述
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '296'
ht-degree: 100%

---

# 令牌概述 {#tokens-overview}

令牌是一种变量，可用于 Marketo 的智能营销活动流程步骤、电子邮件、登陆页面、片段以及 Web 营销活动中。

## 了解默认值 {#understanding-default-values}

在使用令牌时，您还应提供一个默认值。当某位人员在您所引用的字段中没有对应值时，将显示该默认文本。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此示例中，电子邮件将显示为 “Greetings, (first name)” 或 “Greetings, earthling”（默认值）。

![](assets/two.png)

>[!CAUTION]
>
>在使用 Marketo 的电子邮件编辑器时，令牌无法在预览文本中生效。如需在预览文本中使用令牌，必须通过电子邮件模板中的自定义 HTML 来实现。

>[!NOTE]
>
>此列表并非完整清单。Marketo 中的每一个自定义字段都会自动生成对应的令牌。

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
* 如果使用自定义人员字段的显示名称，自定义人员字段同样可以作为令牌使用，例如：`{{lead.Custom Field Name}}`

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
* 如果使用自定义公司字段的显示名称，自定义公司字段同样可以作为令牌使用，例如：`{{Company.Custom Field Name}}`

## 营销活动令牌 {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系统令牌 {#system-tokens}

>[!NOTE]
>
>请参阅[系统令牌词汇表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)，了解有关这些令牌的更多信息。

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
>了解有关基于智能营销活动中所用触发器的[重要时刻令牌](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)的更多详情。

## 项目令牌 {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL My Tokens] {#my-tokens}

[!UICONTROL My Tokens] 在项目中定义，并以 `{{my.` 开头，后接您为该令牌创建的名称。了解有关项目中[我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)的更多信息。

## 成员令牌 {#member-token}

成员令牌用于插入来自集成服务合作伙伴的唯一值。成员令牌的常见用途之一是为网络研讨会参会者生成唯一 URL。每位人员都有一个用于访问网络研讨会的唯一 URL，可通过 `{{member.webinar url}}` 令牌插入。`{{member.webinar url}}` 令牌会自动解析为服务提供方生成的该人员唯一确认 URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>只有当发送该电子邮件的智能营销活动是活动项目的子资源时，`{{member.webinar url}}` 令牌才会生效并填充。
