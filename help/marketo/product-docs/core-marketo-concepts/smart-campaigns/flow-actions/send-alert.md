---
unique-page-id: 1146958
description: 发送警报- Marketo Docs —— 产品文档
title: 发送警报
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# 发送警报{#send-alert}

## 概述{#overview}

Marketo可以向任何人（销售所有者、合作伙伴或其他人）发送包含个人信息的电子邮件警报。 使用&#x200B;**发送警报**&#x200B;流步骤。

![](assets/one-1.png)

## 用法{#usage}

1. 查找并选择要发送的电子邮件。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >您的电子邮件警报必须包含所有标题信息并处于&#x200B;**Approved**&#x200B;状态。

1. 您可以单击预览图标，以确保选择了正确的电子邮件。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >请确保在电子邮件中使用&#x200B;**发送警报信息**&#x200B;令牌。

1. 选择警报收件人。 您可以选择销售责任人或帐户责任人。

   ![](assets/four-2.png)

1. （可选）添加您需要的任何其他电子邮件地址（以逗号或分号分隔）。

   ![](assets/five.png)

   >[!TIP]
   >
   >在触发器活动中，只要值是有效的电子邮件地址，您就可以在&#x200B;**到其他电子邮件**（如`{{lead.Territory Owner}}`或`{{my.Alert Recipient}}`）中使用令牌。 在批处理活动中，**到其他电子邮件**&#x200B;中的令牌将无法工作。

就这样！ 现在您知道如何使用&#x200B;**发送警报**&#x200B;流步骤。

>[!MORELIKETHIS]
>
>[创建电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
