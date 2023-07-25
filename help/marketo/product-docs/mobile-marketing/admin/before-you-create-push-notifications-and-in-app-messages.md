---
unique-page-id: 11376159
description: 在创建推送通知和应用程序内消息之前 — Marketo文档 — 产品文档
title: 在创建推送通知和应用程序内消息之前
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 在创建推送通知和应用程序内消息之前 {#before-you-create-push-notifications-and-in-app-messages}

创建推送通知和应用程序内消息并不困难，但在开始之前，您需要准备好所有内容。 Marketo管理员和移动设备应用程序开发人员应执行以下步骤，准备必要的集成。

1. 首先，Marketo管理员 [添加移动应用程序](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Marketo管理员，然后 [向开发人员发送一个代码片段](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. 开发人员下载SDK，并包括用于的代码片段和其他方法 [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) 或 [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. 默认情况下，应用程序内消息会在应用程序打开时触发。 如果要触发其他事件的消息，例如查看特定页面或按特定按钮时，开发人员需要向代码添加自定义事件(请参阅 [应用程序内消息的自定义事件](#CustomEvents) （如下所示）。

1. 开发人员 [为Android生成服务器API密钥和项目编号](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) 或 [iOS的认证和密码](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) 并将其发送给Marketo管理员。

1. Marketo管理员配置推送通知访问 [使用服务器API密钥(Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) 或 [使用证书(iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Marketo管理员可以很轻松地检查您的推送配置是否已验证。 快走 [此处](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## 应用程序内消息的自定义事件 {#custom-events-for-in-app-messages}

对于应用程序内消息传送，显示触发器设置为 **应用程序打开** 默认情况下。 如果要使用任何自定义事件来触发应用程序内消息的显示(例如， **添加到购物车的点击量**， **“查看设置”页**)，创建所需事件的列表并将其提供给您的移动应用程序开发人员。 然后，开发人员会将自定义事件添加到代码中。 获得批准后，在设置受众时，它们将显示为显示触发器。 **注意**：自定义事件编码审批流程可能需要一些时间才能完成。

在您完成应用程序内消息和推送通知的所有准备工作后，便应该开始了！

>[!MORELIKETHIS]
>
>* [创建应用程序内消息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [创建推送通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
