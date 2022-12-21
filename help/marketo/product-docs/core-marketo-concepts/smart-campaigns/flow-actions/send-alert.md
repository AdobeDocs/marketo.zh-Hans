---
unique-page-id: 1146958
description: 发送警报 — Marketo文档 — 产品文档
title: 发送警报
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# 发送警报 {#send-alert}

## 概述 {#overview}

Marketo可以向任何人（销售所有者、合作伙伴或其他人）发送包含人员信息的电子邮件警报。 使用 **发送警报** 流步骤。

![](assets/one-1.png)

## 使用情况 {#usage}

1. 查找并选择要发送的电子邮件。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >您的电子邮件警报必须包含所有标题信息，并且位于 **已批准** 状态。

1. 您可以单击预览图标，以确保选择了正确的电子邮件。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >请务必使用 **发送警报信息** 令牌。

1. 选择警报收件人。 您可以选择销售责任人或帐户责任人。

   ![](assets/four-2.png)

1. （可选）添加您需要的任何其他电子邮件地址（以逗号分隔或分号分隔）。

   ![](assets/five.png)

   >[!TIP]
   >
   >在触发营销活动中，您可以在 **发送到其他电子邮件** 例如 `{{lead.Territory Owner}}` 或 `{{my.Alert Recipient}}` 只要值是有效的电子邮件地址。 中的令牌 **发送到其他电子邮件** 在批量营销活动中不起作用。

就这样！ 现在，您已了解如何使用 **发送警报** 流步骤。

>[!MORELIKETHIS]
>
>[创建电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
