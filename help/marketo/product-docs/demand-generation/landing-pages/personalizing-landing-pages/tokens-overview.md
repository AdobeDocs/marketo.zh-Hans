---
unique-page-id: 2950799
description: 令牌概述 — Marketo文档 — 产品文档
title: 令牌概述
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 1%

---

# 令牌概述 {#tokens-overview}

令牌是一个变量，可在Marketo智能营销活动流程步骤、电子邮件、登陆页面、代码片段和Web营销活动中使用。

## 了解默认值 {#understanding-default-values}

当您使用令牌时，您还需要提供默认值。 这是显示某人是否不具有您正在引用的字段值的文本。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此示例中，电子邮件会显示“Greetings， (first name)”或“Greetings， earthling”（默认值）。

![](assets/two.png)

>[!CAUTION]
>
>使用Marketo的电子邮件编辑器时，令牌在预标头中无法使用。 要在预标头中使用令牌，必须通过在电子邮件模板中通过您自己的HTML来使用。

>[!NOTE]
>
>这份清单并非详尽无遗。 令牌也是为您在Marketo中拥有的每个自定义字段创建的。

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
* 如果您使用其显示名称（例如，`{{lead.Custom Field Name}}`），自定义人员字段也可正常工作

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
* 如果您使用自定义公司字段的显示名称，例如`{{Company.Custom Field Name}}`

## 营销活动令牌 {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系统令牌 {#system-tokens}

>[!NOTE]
>
>在[系统令牌术语表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)中了解有关这些令牌的更多信息。

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
>根据智能营销活动中使用的触发器，查找有关有趣时刻的[令牌](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)的更多详细信息。

## 项目令牌 {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL My Tokens] {#my-tokens}

[!UICONTROL My Tokens]在项目中定义，以`{{my.`开头，后跟您为令牌创建的名称。 了解有关程序中[我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)的更多信息。

## 成员令牌 {#member-token}

成员令牌用于插入来自集成服务合作伙伴的唯一值。 成员令牌的常见用途是用于网络研讨会参与者的唯一URL。 每个人员都有一个访问网络研讨会的唯一URL，可使用`{{member.webinar url}}`令牌插入该URL。 `{{member.webinar url}}`令牌自动解析服务提供商生成的人员的唯一确认URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>仅当发送电子邮件的智能营销活动是事件程序的子资产时，`{{member.webinar url}}`令牌才会填充。
