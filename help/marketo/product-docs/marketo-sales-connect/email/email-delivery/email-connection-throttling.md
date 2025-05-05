---
description: 电子邮件连接限制 — Marketo文档 — 产品文档
title: 电子邮件连接限制
exl-id: 093f5459-1bbb-45dd-8590-71ea4e1168d4
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 电子邮件连接限制 {#email-connection-throttling}

集成要通过Exchange或Gmail电子邮件提供商发送的Sales Connect帐户，可简化设置并优化一对一销售通信的电子邮件可投放性。 但是，为了保持系统健康和帐户安全，Gmail和Exchange会强制实施电子邮件发送限制。 这些限制可由提供商自行决定增加或减少。

## 概述 {#overview}

电子邮件连接限制允许Sales Connect管理员在使用Gmail或Exchange作为投放渠道时配置电子邮件的发送速率，以便将电子邮件移交给投放渠道提供商的速率不超过实施的限制。

当始终超过限制时，有时可能会被视为投放渠道提供商的可疑行为，从而导致电子邮件失败，有时甚至导致帐户被禁用。

**备注/亮点**

* 用户连接到Gmail或Exchange后自动启用
* 如果要增加或减少推荐中的设置以满足您的需求，可对其进行自定义
* 仅限制通过Gmail或Exchange发送的电子邮件，不会限制自定义投放渠道
* 电子邮件连接限制会将每个单独用户的电子邮件单独排入队列，因为每个用户与其电子邮件提供商都有自己的连接

**配置电子邮件连接限制设置**

1. 单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/email-connection-throttling-1.png)

1. 单击&#x200B;**常规**。

   ![](assets/email-connection-throttling-2.png)

1. 在电子邮件连接限制卡中，输入将发送到电子邮件渠道提供商的电子邮件批次大小。

   ![](assets/email-connection-throttling-3.png)

1. 设置发送每个批次前等待的时间。 在此示例中，我们每45秒选择25封电子邮件。

   ![](assets/email-connection-throttling-4.png)

1. 单击&#x200B;**保存**。

   ![](assets/email-connection-throttling-5.png)

保存更改后，所有用户都将将其电子邮件分批发送到其连接的Gmail或Exchange帐户以进行交付。

## 电子邮件提供商限制 {#email-provider-limits}

**Outlook 365**

商业/企业

* 每天10,000
* 每分钟30次
* 每封电子邮件500个收件人

可在此处[&#128279;](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)找到更多信息。

**Gmail**

* 每天2000个（500个用于试用和标记帐户）
* 每秒2封电子邮件（API限制）
* 每封邮件2,000个收件人（外部收件人最多500个）

可在此处[&#128279;](https://support.google.com/a/answer/166852?hl=en)找到更多信息。

**Microsoft Exchange Server (2010， 2013)**

由于服务器由组织托管，因此限制由组织的IT部门设置。 如有其他信息，请联系网络或系统管理员。

>[!MORELIKETHIS]
>
>* [投放渠道概述](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* Gmail用户的[电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* Outlook用户的[电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
