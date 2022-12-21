---
unique-page-id: 11376159
description: 在创建推送通知和应用程序内消息之前 — Marketo文档 — 产品文档
title: 在创建推送通知和应用程序内消息之前
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 在创建推送通知和应用程序内消息之前 {#before-you-create-push-notifications-and-in-app-messages}

创建推送通知和应用程序内消息并不困难，但您需要先准备好所有内容，然后才能开始。 Marketo管理员和移动设备应用程序开发人员应按照以下步骤来准备必要的集成。

1. 首先，Marketo管理员 [添加移动设备应用程序](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. 然后，Marketo管理员 [向开发人员发送代码段](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. 开发人员下载SDK，其中包括代码片段和其他方法，适用于 [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) 或 [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. 默认情况下，应用程序打开时会触发应用程序内消息。 如果您要为其他事件（例如，在查看特定页面或按下特定按钮时）触发消息，开发人员需要向代码中添加自定义事件(请参阅 [应用程序内消息的自定义事件](#CustomEvents) )。

1. 开发人员 [为Android生成服务器API密钥和项目编号](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) 或 [iOS的认证和密码](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) 并发送给Marketo管理员。

1. Marketo管理员配置推送通知访问权限 [(Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) 或 [(iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Marketo管理员可以轻松检查您的推送配置是否已验证。 快走 [此处](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## 应用程序内消息的自定义事件 {#custom-events-for-in-app-messages}

对于应用程序内消息传送，显示触发器将设置为 **应用程序打开** 默认情况下。 如果您要使用任何自定义事件来触发应用程序内消息的显示(例如， **点击添加到购物车**, **“查看次数设置”页**)，请创建所需事件列表，并将其提供给移动设备应用程序开发人员。 然后，开发人员将自定义事件添加到代码中。 批准后，在设置受众时，它们将显示为显示触发器。 **注意**:自定义事件编码批准过程可能需要一些时间才能完成。

完成应用程序内消息和推送通知的所有准备工作后，便可开始使用！

>[!MORELIKETHIS]
>
>* [创建应用程序内消息](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [创建推送通知](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

