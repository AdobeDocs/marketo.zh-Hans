---
unique-page-id: 2360219
description: 设置自定义DKIM签名 — Marketo文档 — 产品文档
title: 设置自定义DKIM签名
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# 设置自定义DKIM签名 {#set-up-a-custom-dkim-signature}

为确保最高投放能力，我们使用共享的Marketo DKIM签名自动对所有出站邮件进行签名。

>[!NOTE]
>
>您可能需要IT团队的帮助才能完成本文中的一些步骤。

您可以个性化DKIM签名，以反映您选择的域。 这是方法。

1. 转到 **管理员** 中。

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >如果您以旧式方式设置自定义DKIM签名，它将继续工作，并应显示在此处。

1. 单击 **电子邮件**，则 **DKIM** ，最后 **添加域**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. 输入您在Marketo电子邮件中用作发件人地址的域，然后单击 **添加**.

   >[!TIP]
   >
   >如果您在发件人地址中使用其他域，我们将使用Marketo共享DKIM签名。

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. 发送 **主机记录** 和 **TXT值** 给你的IT。 要求他们为您创建记录，并确保该记录传播到与从域关联的所有名称服务器。 Marketo的DKIM验证要求DKIM密钥被传播到与DKIM签名的域关联的所有名称服务器。

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. 确认已创建记录后，返回Marketo，选择您的域，然后单击 **检查DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >如果确认失败，且IT已正确创建记录，则可能是DNS传播的问题。 请稍后重试。

   >[!CAUTION]
   >
   >修改/删除相应的DNS记录将会损害投放能力。 在进行DNS更改之前，请确保删除Marketo中的条目。

   这将对您的电子邮件投放能力提供绝对帮助。 您应该获得记录是否存在且正确的验证。
