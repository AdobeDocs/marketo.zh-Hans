---
description: Marketo取消订阅检查 — Marketo文档 — 产品文档
title: Marketo 取消订阅检查
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 7%

---

# [!UICONTROL Marketo Unsubscribe Check] {#marketo-unsubscribe-check}

[!UICONTROL Marketo Unsubscribe Check]使用您团队与Marketo的连接防止电子邮件发送给在Marketo的潜在客户管理系统中取消订阅的人员。 当销售用户发送带有[!DNL Marketo Sales]的电子邮件时，将对Marketo进行API调用以检查电子邮件ID是否已取消订阅。 如果是，我们将阻止发送电子邮件。

>[!NOTE]
>
>**需要管理员权限**

## 打开 {#turning-it-on}

1. 单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/marketo-unsubscribe-check-1.png)

1. 在[!UICONTROL Admin Settings]下，单击&#x200B;**[!UICONTROL Unsubscribes]**。

   ![](assets/marketo-unsubscribe-check-2.png)

1. 单击 **[!UICONTROL Integrations]** 选项卡。在[!UICONTROL Marketo Unsubscribe Check]部分中，单击滑块以激活检查。

   ![](assets/marketo-unsubscribe-check-3.png)

## 须知事项 {#things-to-know}

Marketo取消订阅检查……

* 不计入API限制中
* 需要建立Marketo连接
* 是全局设置
* 阻止从Web应用程序、电子邮件客户端和[!DNL Salesforce]发送的电子邮件
