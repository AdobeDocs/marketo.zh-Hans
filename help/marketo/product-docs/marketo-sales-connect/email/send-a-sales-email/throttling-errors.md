---
unique-page-id: 14352581
description: 限制错误- Marketo Docs —— 产品文档
title: 限制错误
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# 限制错误{#throttling-errors}

## 已达到文件限制{#file-limit-reached}

如果您通过自己的服务器发送，那么您可以同时发送的电子邮件数量将受到限制。 通过Sales Connect发送时，您可以发送许多电子邮件，但我们会尝试同时发送所有电子邮件。 因此，如果您知道服务器每分钟会切断100封电子邮件，您只需要通过[Web应用程序](https://toutapp.com/login)发送最多100封电子邮件。 否则，由于您的服务器中的电子邮件被限制，电子邮件可能会落在此处。

## 身份验证错误{#authentication-error}

这意味着我们无法验证到SMTP服务器的连接。 您的密码最近更改了，您只需验证新凭据即可。

要执行此操作，请转到“SMTP设置”，您应该看到相同的错误消息。 更新凭据并点击&#x200B;**验证和保存**&#x200B;以查看确认消息。

进入“失败”投放尝试重新发送这些电子邮件。
