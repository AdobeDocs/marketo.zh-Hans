---
unique-page-id: 2360219
description: 设置自定义DKIM签名 — Marketo文档 — 产品文档
title: 设置自定义DKIM签名
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# 设置自定义DKIM签名 {#set-up-a-custom-dkim-signature}

为确保顶级可投放性，我们使用共享的Marketo DKIM签名自动对所有出站邮件进行签名。

>[!NOTE]
>
>您可能需要您的IT团队的帮助来完成本文中的某些步骤。

您可以个性化DKIM签名以反映您选择的域。 具体方法如下。

1. 转到 **管理员** 部分。

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >如果您以传统方式设置自定义DKIM签名，它将继续工作，并且应该在此处显示。

1. 单击 **电子邮件**，然后 **DKIM** 选项卡，最后 **添加域**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. 输入将在Marketo电子邮件中使用的域作为发件人地址，然后单击 **添加**.

   >[!TIP]
   >
   >如果您在发件人地址中使用其他域，我们将使用Marketo共享DKIM签名。

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. 发送 **主机记录** 和 **TXT值** 到你的IT。 要求他们为您创建记录，并确保该记录传播到与来自域关联的所有名称服务器。 Marketo的DKIM验证要求将DKIM密钥传播到与DKIM签名的域关联的所有名称服务器。

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. 确认创建了记录后，请返回Marketo并选择您的域，然后单击 **检查DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >如果确认失败，并且您的IT部门正确创建了记录，则可能与DNS传播有关。 请稍后重试。

   >[!CAUTION]
   >
   >修改/删除相应的DNS记录将导致有害的可投放性。 确保在进行DNS更改之前删除Marketo中的条目。

   这绝对有助于您的电子邮件可投放性。 您应该获得确认，记录存在并且正确。
