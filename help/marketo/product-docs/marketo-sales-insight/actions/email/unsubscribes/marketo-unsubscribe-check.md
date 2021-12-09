---
description: Marketo取消订阅检查 — Marketo文档 — 产品文档
title: Marketo取消订阅检查
hide: true
hidefromtoc: true
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Marketo取消订阅检查 {#marketo-unsubscribe-check}

Marketo取消订阅检查会使用您的团队与Marketo的连接来阻止电子邮件发送给Marketo潜在客户管理系统中已取消订阅的用户。 当销售用户通过Marketo Sales发送电子邮件时，将向Marketo发送API调用，以检查电子邮件ID是否已取消订阅。 如果是，我们将阻止发送电子邮件。

>[!NOTE]
>
>**需要管理员权限**

## 打开它 {#turning-it-on}

1. 单击齿轮图标，然后选择 **设置**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. 在“管理员设置”下，单击 **取消订阅**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. 单击 **集成** 选项卡。 在Marketo取消订阅检查部分，单击滑块以激活检查。

   ![](assets/marketo-unsubscribe-check-3.png)

## 注意事项 {#things-to-know}

Marketo取消订阅检查……

* 不计入API限制
* 需要建立Marketo连接
* 是全局设置
* 阻止从Web应用程序、电子邮件客户端和Salesforce发送的电子邮件
