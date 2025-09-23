---
unique-page-id: 1147356
description: 了解电子邮件事件日志 — Marketo文档 — 产品文档
title: 了解电子邮件事件日志
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 3%

---

# 了解电子邮件事件日志 {#understanding-email-event-logging}

在发送电子邮件时，Marketo会将不同的数据点记录到人员的活动日志中。 以下是基本部分。

| 活动 | 描述 |
|---|---|
| [!UICONTROL Sent] | 每次从Marketo服务器发送电子邮件时都会记录，而不管该电子邮件是否实际发送。 退回的电子邮件仍记录为“已发送”。 |
| [!UICONTROL Delivered] | 每次收件人邮件服务器接受电子邮件时都会记录。 这并不意味着它避免了垃圾邮件过滤器。 每个已发送电子邮件只能有1个投放。 |
| [!UICONTROL Hard Bounced] | 部分硬退回是垃圾邮件阻止的结果，因此在任何营销活动中，我们将不会在24小时内尝试向该用户发送电子邮件。 其他硬退信（如不存在收件箱）是永久性的，我们将永远不再通过任何营销活动向此人发送电子邮件。 |
| [!UICONTROL Soft Bounced] | 在服务器响应不明确、邮箱已满或服务器出现一般问题时记录。 我们会为这些用户设置24-36小时的重试逻辑，以便将来可能的投放。 这不会取消此人发送其他邮件的资格。 |
| [!UICONTROL Opened] | 当收件人查看包含“未阻止”图像的电子邮件时记录。 每个电子邮件、每个人和每个智能营销活动仅记录一个打开事件。 如果访客从收件箱中打开同一电子邮件两次，则记录不会超过一次。 |
| [!UICONTROL Clicked] | 每次将电子邮件中经过修饰的URL加载到浏览器中时（单击链接的结果），都会进行记录。 通常这是收件人点击，但也可能是剪切/粘贴。 |
| [!UICONTROL Unsubscribed] | 在人员单击电子邮件的取消订阅链接并提交取消订阅表单时记录。 |

>[!CAUTION]
>
>如果同一电子邮件从同一营销活动两次发送给同一个人，则最多将记录1次&#x200B;**[!UICONTROL Opened]**&#x200B;事件。
