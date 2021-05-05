---
unique-page-id: 2950799
description: 令牌概述 — Marketo Docs — 产品文档
title: 令牌概述
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
translation-type: tm+mt
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 令牌概述{#tokens-overview}

令牌是一个变量，可用于Marketo智能活动流步骤、电子邮件、登陆页、片段和Web活动。

## 了解默认值{#understanding-default-values}

使用令牌时，您还希望提供默认值。 这是显示人员是否没有您引用的字段值的文本。

![](assets/image2014-12-2-13-3a16-3a48.png)

在此示例中，电子邮件将显示“Greetings，(first name)”或“Greetings， earthling”（默认值）。

![](assets/two.png)

>[!CAUTION]
>
>使用Marketo的电子邮件编辑器时，令牌在头中不起作用。 要使用标题中的标记，它必须通过电子邮件模板中您自己的HTML进行。

>[!NOTE]
>
>此列表并非详尽无遗。 还会为您在Marketo中拥有的每个自定义字段创建令牌。

## 人物令牌{#person-tokens}

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
* 如果您使用自定义人员字段的显示名称（例如`{{lead.Custom Field Name}}`），则自定义人员字段也会正常工作

## 公司令牌{#company-tokens}

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
* 如果您使用自定义公司字段的显示名称（例如），则自定义字段也会正常工作。`{{Company.Custom Field Name}}`

## 活动令牌{#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## 系统令牌{#system-tokens}

>[!NOTE]
>
>在[系统令牌词汇表](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md)中了解有关这些令牌的更多信息。

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## 触发器令牌{#trigger-tokens}

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
>根据智能活动中使用的触发器，查找有关[令牌的更多详细信息，以获得有趣的瞬间](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)。

## 项目令牌{#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## 我的令牌{#my-tokens}

我的令牌是在项目中定义的，以`{{my.`开头，后跟您为令牌创建的名称。 了解有关[项目](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)中我的令牌的更多信息。

## 成员令牌{#member-token}

会员令牌用于插入集成服务合作伙伴的唯一值。 会员令牌的常用功能是网络研讨会与会者的唯一URL。 每个人都有一个唯一的URL，用于访问可以使用`{{member.webinar url}}`令牌插入的网络研讨会。 `{{member.webinar url}}`标记会自动解析由服务提供商生成的个人唯一确认URL。

* `{{member.webinar url}}`

>[!CAUTION]
>
>`{{member.webinar url}}`令牌仅在发送电子邮件的智能活动是事件项目的子资产时填充。
