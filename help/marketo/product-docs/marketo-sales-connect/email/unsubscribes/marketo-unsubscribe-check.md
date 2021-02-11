---
unique-page-id: 18317340
description: Marketo取消订阅检查- Marketo文档——产品文档
title: Marketo取消订阅检查
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Marketo取消订阅检查{#marketo-unsubscribe-check}

Marketo取消订阅检查使用您的团队与Market的连接来阻止电子邮件发送给Marketo的潜在客户管理系统中未订阅的用户。 当销售用户通过Sales Connect发送电子邮件时，将向Market发出API调用，以检查电子邮件ID是否取消订阅。 如果是，我们将阻止发送电子邮件。

>[!NOTE]
>
>**需要管理员权限**

## 打开{#turning-it-on}

1. 在Web应用程序中，单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/one-2.png)

1. 在“管理员设置”下，单击&#x200B;**取消订阅**。

   ![](assets/two-3.png)

1. 单击&#x200B;**集成**。

   ![](assets/three-3.png)

1. 在“Marketo取消订阅检查”部分，单击滑块以激活检查。

   ![](assets/four-2.png)

## {#things-to-know}的注意事项

Marketo取消订阅检查……

* 不计入API限制
* 需要建立Marketo连接
* 是全局设置
* 阻止从Web应用程序、电子邮件客户端和Salesforce发送的电子邮件
