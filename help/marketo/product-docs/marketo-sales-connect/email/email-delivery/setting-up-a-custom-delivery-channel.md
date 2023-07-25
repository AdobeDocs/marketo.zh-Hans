---
unique-page-id: 14746470
description: 设置自定义投放渠道 — Marketo文档 — 产品文档
title: 设置自定义投放渠道
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# 设置自定义投放渠道 {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect允许您与自定义SMTP服务器集成，以投放电子邮件。 对于那些不想从Gmail或Exchange投放渠道发送批量电子邮件的人来说，这是一个很好的选项。

用户可以设置自定义SMTP服务器以供其单独使用，管理员也可以设置一个要在实例中的所有Sales Connect用户之间共享的Team SMTP。

>[!NOTE]
>
>* 除了设置SMTP服务器外， [必须验证电子邮件身份](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) 才能发送电子邮件。
>* 我们建议您与IT团队或SMTP服务器供应商合作，以获取SMTP服务器的正确服务器凭据。
>* 无法使用SMTP服务器凭据连接Gmail和Exchange服务器。 请使用我们的电子邮件连接服务与这些提供商集成。

## 自定义SMTP {#custom-smtp}

1. 登录到 [Web应用程序](https://toutapp.com/login)，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. 在“我的帐户”下，单击 **电子邮件设置**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. 单击 **自定义投放渠道**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. 输入您的SMTP服务器凭据，然后单击 **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >如果这是您唯一的投放渠道，则会自动将其分配给您的所有电子邮件身份，而您已经完成此操作。 如果这不是您唯一的投放渠道，请继续执行步骤5。

1. 当仍处于“电子邮件设置”中时，单击 **地址和签名**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. 查找要为其选择投放渠道的电子邮件身份，然后单击 **选择投放渠道**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. 在“可投放性”卡中，单击 **编辑**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. 单击渠道下拉列表，然后选择您刚刚添加的自定义投放渠道。 单击 **保存**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >如果您的团队管理员设置了Team SMTP Server，它将仅自动应用于您的默认电子邮件标识，并且可用作您的其他电子邮件标识的选项。

## Team SMTP服务器 {#team-smtp-server}

>[!NOTE]
>
>**需要管理员权限**

1. 登录到 [Web应用程序](https://toutapp.com/login)，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. 在管理设置下，单击 **常规**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. 单击 **团队交付渠道**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. 输入您的SMTP服务器凭据，然后单击 **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Team SMTP服务器将是所有团队成员默认电子邮件标识的默认投放渠道。 此外，它还将作为所有其他电子邮件标识的投放渠道选项提供。

   >[!MORELIKETHIS]
   >
   >* [Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
