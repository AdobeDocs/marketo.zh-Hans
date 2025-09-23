---
unique-page-id: 11376159
description: 在创建推送通知和应用程序内消息之前 — Marketo文档 — 产品文档
title: 在创建推送通知和应用程序内消息之前
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 4%

---

# 在创建推送通知和应用程序内消息之前 {#before-you-create-push-notifications-and-in-app-messages}

创建推送通知和应用程序内消息并不困难，但在开始之前，您需要准备好所有内容。 Marketo管理员和移动设备应用程序开发人员应执行以下步骤来准备必要的集成。

1. 首先，Marketo管理员[添加移动应用](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md)。

1. 然后Marketo管理员[向开发人员](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md)发送一个代码片段。

1. 开发人员下载适用于[Android](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)或[iOS](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios)的SDK，并包含代码片段和其他方法。

1. 默认情况下，应用程序内消息会在应用程序打开时触发。 如果要触发其他事件的消息，例如查看特定页面或按下特定按钮时，开发人员需要向代码添加自定义事件（请参阅下面的[应用程序内消息的自定义事件](#CustomEvents)）。

1. 开发人员[为Android](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)或[iOS](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios)生成服务器API密钥和项目编号，并将其发送给Marketo管理员。

1. Marketo管理员使用服务器API密钥(Android) [配置推送通知访问](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md)，或使用证书(iOS) [配置](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)。

>[!TIP]
>
>Marketo管理员可以轻松检查推送配置是否已验证。 只需[此处](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md)。

## 应用程序内消息的自定义事件 {#custom-events-for-in-app-messages}

对于应用程序内消息传送，显示触发器默认设置为&#x200B;**[!UICONTROL App Open]**。 如果要使用任何自定义事件来触发应用内消息的显示（例如，**单击“添加到购物车”**、**查看设置页面**），请创建所需事件的列表，并将其提供给您的移动应用开发人员。 然后，开发人员会将自定义事件添加到代码中。 获得批准后，在设置受众时，它们将显示为显示触发器。 **注意**：自定义事件编码审批流程可能需要一些时间才能完成。

在您完成应用程序内消息和推送通知的所有准备工作后，便应该开始了！

>[!MORELIKETHIS]
>
>* [创建应用程序内消息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [创建推送通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
