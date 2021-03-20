---
unique-page-id: 14746470
description: 设置自定义投放渠道- Marketo Docs — 产品文档
title: 设置自定义投放渠道
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# 设置自定义投放渠道{#setting-up-a-custom-delivery-channel}

Marketo Sales Connect允许您与自定义SMTP服务器集成，以投放电子邮件。 对于那些不想从Gmail或Exchange投放渠道发送批量电子邮件的用户来说，这是一个绝佳的选择。

用户可以设置自定义SMTP服务器以用于自己的个人用法，或者管理员可以设置要在实例中的所有Sales Connect用户之间共享的团队SMTP。

>[!NOTE]
>
>* 除设置SMTP服务器外，您的[电子邮件标识必须经过](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)验证，然后才能发送电子邮件。
>* 我们建议与您的IT团队或SMTP服务器供应商合作，为您的SMTP服务器获取正确的服务器凭据。
>* 您无法使用SMTP服务器凭据连接Gmail和Exchange服务器。 请使用我们的电子邮件连接服务与这些提供商集成。


## 自定义SMTP {#custom-smtp}

1. 登录到[Web应用程序](https://toutapp.com/login)，单击右上方的齿轮图标并选择&#x200B;**设置**。

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. 在“我的帐户”下，单击&#x200B;**电子邮件设置**。

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. 单击&#x200B;**自定义投放渠道**。

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. 输入您的SMTP服务器凭据，然后单击&#x200B;**Connect**。

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >如果这是您唯一的投放渠道，则会自动将其分配给您的所有电子邮件身份，您就可以在此处完成。 如果这不是您唯一的投放渠道，请继续执行步骤5。

1. 仍在“电子邮件设置”中时，单击&#x200B;**地址和签名**。

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. 查找要为其选择投放渠道的电子邮件标识，然后单击&#x200B;**选择投放渠道**。

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. 在“可交付性卡”中，单击&#x200B;**编辑**。

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. 单击“渠道”下拉框，然后选择您刚添加的自定义投放渠道。 单击&#x200B;**保存**。

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >如果您的团队管理员设置了团队SMTP服务器，它将自动仅应用于您的默认电子邮件标识，并可作为其他电子邮件标识的选项。

## 团队SMTP服务器{#team-smtp-server}

>[!NOTE]
>
>**需要管理权限**

1. 登录到[Web应用程序](https://toutapp.com/login)，单击右上方的齿轮图标并选择&#x200B;**设置**。

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. 在“管理设置”下，单击&#x200B;**常规**。

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. 单击&#x200B;**团队投放渠道**。

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. 输入您的SMTP服务器凭据，然后单击&#x200B;**Connect**。

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >团队SMTP服务器将是所有团队成员默认电子邮件标识的默认投放渠道。 此外，它还可作为所有其他电子邮件身份的投放渠道选项。

   >[!MORELIKETHIS]
   >
   >* [针对Gmail用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
      >
      >
   * [Outlook用户的电子邮件连接](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

