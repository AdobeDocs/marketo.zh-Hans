---
unique-page-id: 11376159
description: 在创建推送通知和应用程序内消息- Marketo Docs —— 产品文档之前
title: 在创建推送通知和应用程序内消息之前
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# 在创建推送通知和应用程序内消息之前 {#before-you-create-push-notifications-and-in-app-messages}

创建推送通知和应用程序内消息并不困难，但您需要准备好一切，然后才能进行开始。 营销人员管理员和移动应用程序开发人员应按照以下步骤准备必要的集成。

1. 首先，Marketo Admin添加 [了移动应用程序](add-a-mobile-app.md)
1. Marketo管理员随后 [会向开发人员发送代码片断](send-sdk-code-to-a-developer.md)
1. 开发人员下载SDK，包括Android或iOS的片段和其 [他方](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/)[法](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. 默认情况下，应用程序打开时将触发应用程序内消息。 如果您要为其他事件触发消息，例如当查看特定页面或按下特定按钮时，开发人员需要向代码中添加自定义事件(请参阅下 [面的应用程序内消息的自定义事件](#CustomEvents) )
1. 开发人 [员为Android生成服务器API密钥和项目编号](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) , [或为iOS生成证书和密码](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) ，并将其发送给Marketo Admin
1. 营销人员管理员使用服 [务器API密钥(Android)或证书](configure-mobile-app-android-push-access.md) ( [iOS)配置推送通知访问](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>营销人员管理员可轻松检查您的推送配置是否经过验证。 就去 [这](verify-push-configuration.md)。

## 应用程序内消息的自定义事件 {#custom-events-for-in-app-messages}

对于应用程序内消息传递，默认情况下，显示触发器 **设置为** “应用程序打开”。 如果要使用任何自定义事件触发应用程序内消息的显示(例如， **单击“添加到购物车**”、 **“视图设置页面”**)，请创建所需事件的列表，并将其提供给您的移动应用程序开发人员。 开发人员随后将自定义事件添加到代码中。 批准后，在设置受众时，它们将显示为显示触发器。 **注意**:自定义事件编码批准过程可能需要一些时间才能完成。

完成所有应用程序内消息和推送通知准备工作后，该开始了！

>[!MORELIKETHIS]
>
>* [创建应用程序内消息](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [创建推送通知](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



