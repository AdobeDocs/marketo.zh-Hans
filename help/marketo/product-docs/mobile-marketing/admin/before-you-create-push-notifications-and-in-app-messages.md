---
unique-page-id: 11376159
description: 在创建推送通知和应用程序内消息 — Marketo Docs — 产品文档之前
title: 在创建推送通知和应用程序内消息之前
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# 创建推送通知和应用程序内消息{#before-you-create-push-notifications-and-in-app-messages}之前

创建推送通知和应用程序内消息并不困难，但您需要准备好所有内容，然后才能进行开始。 营销人员管理员和移动应用程序开发人员应按照以下步骤准备必要的集成。

1. 首先，Marketo管理员[添加移动应用程序](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md)。

1. 然后，Marketo管理员[向开发人员](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md)发送代码片断。

1. 开发人员下载SDK，包括针对[Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/)或[iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)的片段和其他方法。

1. 默认情况下，应用程序打开时将触发应用程序内消息。 如果要触发其他事件的消息，例如查看特定页面或按下特定按钮时，开发人员需要向代码中添加自定义事件(请参阅下面的[应用程序内消息的自定义事件](#CustomEvents))。

1. 开发人员[生成Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/)或[的证书和密码的服务器API密钥和项目号，并将其发送给Marketo管理员。](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/)

1. Marketo管理员使用服务器API密钥(Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md)或使用证书(iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)配置推送通知访问[。[

>[!TIP]
>
>Marketo Admin可轻松检查您的推送配置是否已验证。 只需转到[此处](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md)。

## 应用程序内消息{#custom-events-for-in-app-messages}的自定义事件

对于应用程序内消息传递，默认情况下，显示触发器设置为&#x200B;**App Open**。 如果您要使用任何自定义事件触发应用程序内消息的显示(例如，**单击添加到购物车**、**视图设置页面**)，请创建所需事件的列表，并将其提供给您的移动应用程序开发人员。 然后，开发人员将自定义事件添加到代码中。 在批准后，在设置受众时，它们会显示为显示触发器。 **注意**:自定义事件编码批准过程可能需要一些时间才能完成。

完成应用程序内消息和推送通知的所有准备工作后，该开始了！

>[!MORELIKETHIS]
>
>* [创建应用程序内消息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
   >
   >
* [创建推送通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

