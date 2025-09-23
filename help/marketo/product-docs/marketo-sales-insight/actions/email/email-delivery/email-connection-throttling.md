---
description: 电子邮件连接限制 — Marketo文档 — 产品文档
title: 电子邮件连接节流
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# 电子邮件连接节流 {#email-connection-throttling}

集成要通过[!DNL Sales Connect]或Gmail电子邮件提供商发送的[!DNL Exchange]帐户，可简化设置并优化1:1销售通信的电子邮件可投放性。 但是，为了保持系统健康和帐户安全，Gmail和[!DNL Exchange]强制执行电子邮件发送限制。 这些限制可由提供商自行决定增加或减少。

## 概述 {#overview}

电子邮件连接限制允许Sales Connect管理员在使用Gmail或Exchange作为投放渠道时配置电子邮件的发送速率，以便将电子邮件移交给投放渠道提供商的速率不超过实施的限制。

当始终超过限制时，有时可能会被视为投放渠道提供商的可疑行为，从而导致电子邮件失败，有时甚至导致帐户被禁用。

## 注意事项 {#things-to-note}

* 当用户连接到Gmail或[!DNL Exchange]时自动启用
* 如果要增加或减少推荐中的设置以满足您的需求，可对其进行自定义
* 仅限制通过Gmail或[!DNL Exchange]发送的电子邮件，不会限制自定义投放渠道
* 电子邮件连接限制会将每个单独用户的电子邮件单独排入队列，因为每个用户与其电子邮件提供商都有自己的连接

## 配置电子邮件连接限制设置 {#configuring}

1. 单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/email-connection-throttling-1.png)

1. 在[!UICONTROL Admin Settings]下，单击&#x200B;**[!UICONTROL General]**。

   ![](assets/email-connection-throttling-2.png)

1. 在右侧的电子邮件连接限制卡中，单击&#x200B;**[!UICONTROL Enable Email Throttling]**&#x200B;滑块。

   ![](assets/email-connection-throttling-3.png)

1. 在右侧的电子邮件连接限制卡中，输入将发送到电子邮件渠道提供商的电子邮件批次大小。

   ![](assets/email-connection-throttling-4.png)

1. 设置发送每个批次前等待的时间。 在此示例中，我们每45秒选择25封电子邮件。

   ![](assets/email-connection-throttling-5.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/email-connection-throttling-6.png)

保存更改后，所有用户的电子邮件将分批发送到其连接的Gmail或[!DNL Exchange]帐户以进行传递。

## 电子邮件提供商限制 {#email-provider-limits}

### [!DNL Outlook 365] {#outlook}

商业/企业

* 每天10,000
* 每分钟30次
* 每封电子邮件500个收件人

可在此处[找到更多信息](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)。

### Gmail {#gmail}

* 每天2000个（500个用于试用和标记帐户）
* 每秒2封电子邮件（API限制）
* 每封邮件2,000个收件人（外部收件人最多500个）

可在此处[找到更多信息](https://support.google.com/a/answer/166852?hl=en)。

### [!DNL Microsoft Exchange Server (2010, 2013)] {#microsoft-exchange}

由于服务器由组织托管，因此限制由组织的IT部门设置。 如有其他信息，请联系网络或系统管理员。

>[!MORELIKETHIS]
>
>* [投放渠道概述](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* Gmail用户的[电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* Outlook用户的[电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
