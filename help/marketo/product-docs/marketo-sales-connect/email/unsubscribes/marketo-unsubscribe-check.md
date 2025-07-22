---
unique-page-id: 18317340
description: Marketo取消订阅检查 — Marketo文档 — 产品文档
title: Marketo取消订阅检查
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Marketo取消订阅检查 {#marketo-unsubscribe-check}

[!UICONTROL Marketo Unsubscribe Check]使用您团队与Marketo的连接防止电子邮件发送给在Marketo的潜在客户管理系统中取消订阅的人员。 当销售用户发送带有[!DNL Sales Connect]的电子邮件时，将对Marketo进行API调用以检查电子邮件ID是否已取消订阅。 如果是，我们将阻止发送电子邮件。

>[!NOTE]
>
>**需要管理员权限**

## 打开 {#turning-it-on}

1. 在Web应用程序中，单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-2.png)

1. 在[!UICONTROL Admin Settings]下，单击&#x200B;**[!UICONTROL Unsubscribes]**。

   ![](assets/two-3.png)

1. 单击 **[!UICONTROL Integrations]**。

   ![](assets/three-3.png)

1. 在[!UICONTROL Marketo Unsubscribe Check]部分中，单击滑块以激活检查。

   ![](assets/four-2.png)

## 注意事项 {#things-to-know}

Marketo取消订阅检查……

* 不计入API限制中
* 需要建立Marketo连接
* 是全局设置
* 阻止从Web应用程序、电子邮件客户端和Salesforce发送的电子邮件
* 将记录失败的电子邮件，或阻止用户在尝试发送所有工作流（电子邮件插件发送、单个发送、销售活动发送、多个选择和发送）时发送，但[组电子邮件](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md)除外，我们将阻止以静默方式发送电子邮件
