---
description: 电子邮件连接限制 — Marketo文档 — 产品文档
title: 电子邮件连接限制
exl-id: 093f5459-1bbb-45dd-8590-71ea4e1168d4
source-git-commit: ad7b222c2da937474565729a09a559fbcd722280
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 电子邮件连接限制 {#email-connection-throttling}

将您的Sales Connect帐户集成到通过Exchange或Gmail电子邮件提供商发送，可简化设置并优化电子邮件投放能力，以实现1:1销售通信。 但是，为了保持系统健康和帐户安全，Gmail和Exchange强制实施电子邮件发送限制。 这些限额可由提供者酌情增加或减少。

## 概述 {#overview}

Email Connection Throttling允许Sales Connect管理员在使用Gmail或Exchange作为您的投放渠道时配置电子邮件的发送率，以便将电子邮件传递给投放渠道提供商的速率不会超出强制限制。

当始终超出限制时，有时可能会被视为来自投放渠道提供商的可疑行为，导致电子邮件失败，有时甚至会禁用帐户。

**注释/亮点**

* 用户连接到Gmail或Exchange后自动启用
* 如果您希望增加或减少推荐的设置以满足您的需求，则可以自定义
* 只有通过Gmail或Exchange发送的限制电子邮件，才不会限制自定义投放渠道
* Email Connection限制会将每个用户单独发送的电子邮件排入队列，因为每个用户都有其与其电子邮件提供商的连接

**配置电子邮件连接限制设置**

1. 单击齿轮图标，然后选择 **设置**.

   ![](assets/email-connection-throttling-1.png)

1. 单击 **常规**.

   ![](assets/email-connection-throttling-2.png)

1. 在“电子邮件连接限制”卡中，输入要发送到电子邮件渠道提供商的电子邮件的批量大小。

   ![](assets/email-connection-throttling-3.png)

1. 设置在发送每个批次之前等待的时间。 在本例中，我们每45秒选择25封电子邮件。

   ![](assets/email-connection-throttling-4.png)

1. 单击 **保存**.

   ![](assets/email-connection-throttling-5.png)

保存更改后，所有用户都会将其电子邮件分批发送到其连接的Gmail或Exchange帐户进行交付。

## 电子邮件提供程序限制 {#email-provider-limits}

**Outlook 365**

企业/企业

* 每天10,000
* 每分钟30人
* 每封电子邮件有500位收件人

更多信息 [可在此处找到](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 每天2000人（500人用于试用帐户和已标记帐户）
* 每秒2封电子邮件（API限制）
* 每封邮件2,000个收件人（外部收件人最多500个）

更多信息 [可在此处找到](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server(2010、2013)**

由组织的IT部门设置限制，因为服务器由组织托管。 如需其他信息，请联系网络或系统管理员。

>[!MORELIKETHIS]
>
>* [投放渠道概述](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [面向Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [面向Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

