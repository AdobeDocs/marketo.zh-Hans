---
unique-page-id: 1146958
description: 发送警报- Marketo Docs —— 产品文档
title: 发送警报
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# 发送警报 {#send-alert}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 概述 {#overview}

Marketo可以向任何人（销售所有者、合作伙伴或其他人）发送包含个人信息的电子邮件警报。 使用发 **送警报** 流步骤。

![](assets/one-1.png)

## 使用情况 {#usage}

1. 查找并选择要发送的电子邮件。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >您的电子邮件警报必须包含所有标题信息并处于“已批 **准** ”状态。

1. 您可以单击预览图标，以确保选择了正确的电子邮件。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >请确保在电子邮件 **中使用“发送警报** ”信息令牌。

1. 选择警报收件人。 您可以选择销售责任人或帐户责任人。

   ![](assets/four-2.png)

1. （可选）添加您需要的任何其他电子邮件地址（以逗号或分号分隔）。

   ![](assets/five.png)

   >[!TIP]
   >
   >在触发活动中，您可以在“发送至 **其他电子邮件** ”中使 `{{lead.Territory Owner}}` 用令牌 `{{my.Alert Recipient}}` ，或者只要这些值是有效的电子邮件地址。 在批 **处理活动中** ,“发送到其他电子邮件”中的令牌无法工作。

就这样！ 现在您知道如何使用“发送 **警报流** ”步骤。

>[!MORELIKETHIS]
>
>[创建电子邮件](../../../../product-docs/email-marketing/general/creating-an-email/create-an-email.md)

