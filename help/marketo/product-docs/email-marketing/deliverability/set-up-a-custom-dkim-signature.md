---
unique-page-id: 2360219
description: 设置自定义DKIM签名- Marketo Docs —— 产品文档
title: 设置自定义DKIM签名
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# 设置自定义DKIM签名{#set-up-a-custom-dkim-signature}

为了确保一流的交付能力，我们使用共享的Marketo DKIM签名自动签署所有出站邮件。

>[!NOTE]
>
>您可能需要IT团队的帮助才能完成本文中的一些步骤。

您可以个性化DKIM签名，以反映您选择的域。 这是方法。

1. 转至&#x200B;**Admin**&#x200B;部分。

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >
   >如果您以传统方式设置自定义DKIM签名，它将继续工作，并应显示在此处。

1. 单击&#x200B;**电子邮件**，然后单击&#x200B;**DKIM**&#x200B;选项卡，最后单击&#x200B;**添加域**。

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. 输入您将在Marketo电子邮件中用作发件人地址的域，然后单击&#x200B;**添加**。

   >[!TIP]
   >
   >
   >如果您在发件人地址中使用其他域，我们将使用Marketto共享DKIM签名。

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. 将&#x200B;**主机记录**&#x200B;和&#x200B;**TXT值**&#x200B;发送给您的IT人员。 要求他们为您创建记录，并确保它传播到与from域关联的所有命名空间。 Marketo的DKIM验证要求DKIM密钥传播到与正在DKIM签名的域相关的所有命名空间器。

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. 确认已创建记录后，返回Marketo，选择您的域，然后单击&#x200B;**检查DNS**。

   ![](assets/check.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >如果确认失败，且您的IT人员已正确创建记录，则可能是DNS传播的问题。 稍后再试。

   >[!CAUTION]
   >
   >
   >修改／删除相应的DNS记录将会损害交付能力。 在进行DNS更改之前，请确保删除Marketo中的条目。

   这将完全有助于您提供电子邮件。 您应当获得验证，确认记录已存在且正确。

