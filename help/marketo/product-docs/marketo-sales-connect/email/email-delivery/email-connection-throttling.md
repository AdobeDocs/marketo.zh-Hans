---
description: 电子邮件连接限制 — Marketo Docs — 产品文档
title: 电子邮件连接限制
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---


# 电子邮件连接限制{#email-connection-throttling}

将您的Sales Connect帐户集成到通过Exchange或Gmail电子邮件提供商发送，优惠可以简化设置并优化电子邮件的发送能力，以实现一对一的销售通信。 然而，为了保持系统健康和帐户安全，Gmail和Exchange强制实施电子邮件发送限制。 供应商可自行决定增加或减少这些限额。

## 电子邮件连接限制（测试版）{#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>此功能当前在测试版中。 要加入此测试版，请联系您的客户成功经理。

Email Connection Throttling允许Sales Connect管理员在使用Gmail或Exchange作为投放渠道时配置电子邮件的发送速率，以便将电子邮件转交给投放渠道提供商的速率不超过强制限制。

当限制持续超过时，有时会被视为来自投放渠道提供商的可疑行为，导致电子邮件失败，有时甚至帐户被禁用。

**附注/亮点**

* 用户连接到Gmail或Exchange时自动启用
* 如果您希望增加或减少推荐的设置以满足您的需求，可以进行自定义
* 只限制通过Gmail或Exchange发送的电子邮件，不限制自定义投放渠道
* “电子邮件连接”限制将每个用户的电子邮件分别排队，因为每个用户都与其电子邮件提供商有自己的连接

**配置电子邮件连接限制设置**

1. 单击齿轮图标，然后选择&#x200B;**设置**。

   ![](assets/email-connection-throttling-1.png)

1. 单击&#x200B;**常规**。

   ![](assets/email-connection-throttling-2.png)

1. 在“电子邮件连接限制”卡中，输入要发送给电子邮件渠道提供商的电子邮件的所需批量大小。

   ![](assets/email-connection-throttling-3.png)

1. 设置发送每个批之前等待的时间。 在此示例中，我们每45秒选择25封电子邮件。

   ![](assets/email-connection-throttling-4.png)

1. 单击&#x200B;**保存**。

   ![](assets/email-connection-throttling-5.png)

保存更改后，所有用户都会将电子邮件批量发送到其连接的Gmail或Exchange帐户以进行投放。

## 电子邮件提供者限制{#email-provider-limits}

**Outlook 365**

企业/企业

* 每天10,000
* 每分钟30人
* 每封电子邮件500个收件人

更多信息[可在此处](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)找到。

**Gmail**

* 每天2000（500用于试用帐户和已标记帐户）
* 每秒2封电子邮件（API限制）
* 每封邮件2,000次收件人(外部收件人最多500次)

更多信息[可在此处](https://support.google.com/a/answer/166852?hl=en)找到。

**Microsoft Exchange Server(2010、2013)**

限制由组织的IT部门设置，因为服务器由组织托管。 如果适用，请与网络或系统管理员联系以了解详细信息。

>[!MORELIKETHIS]
>
>* [投放渠道概述](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [针对Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

