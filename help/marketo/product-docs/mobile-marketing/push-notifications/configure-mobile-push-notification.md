---
unique-page-id: 7512454
description: 配置移动推送通知 — Marketo Docs — 产品文档
title: 配置移动推送通知
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# 配置移动推送通知{#configure-mobile-push-notification}

1. 转到“营销活动”区域。

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. 选择您的推送资源，然后单击&#x200B;**编辑草稿**。

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. 转至&#x200B;**Setup**。

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. 选择所需的应用程序。 默认情况下，Android和Apple平台处于启用状态。

   ![](assets/image2016-8-23-16-3a53-3a33.png)

   如果您的推送消息仅应用于一个平台（例如，iPhone的情况），则可以通过将其选择器滑动到“已禁用”来排除另一个平台。

   ![](assets/image2016-8-23-16-3a41-3a48.png)

   单击“下一步”。

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. 输入消息文本或选择标记图标以添加标记。 然后，选择&#x200B;**点按操作**。

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >如果平台处于启用状态，则平台将显示在电话屏幕的左侧。 选择后，它以颜色显示。

   >[!NOTE]
   >
   >**定义**
   >
   >
   >**点击操作有三种类型：**
   >
   >
   >**启动应用** - **此操** 作在点击通知后暂停应用程序的主页。**客** 户使用深层链接打开应用程序或您具有该链接的任何其他应用程序的其他区域(有关详细信息， [请参阅](#Deeplink) 下面的深层链接URI)。
   >
   >
   >**登陆页**  — 将您带到指定的Marketo登陆页。
   >
   >
   >**外部URL**  — 将您带到非营销登陆页。

   要为自定义点击操作插入深层链接，请单击“自定义”，然后在字段中输入[深层链接URI](#Deeplink)。

   ![](assets/image2016-7-28-16-3a19-3a13.png)

   要插入令牌，请选择一个令牌，输入默认值，然后单击插入。

   >[!NOTE]
   >
   >将光标置于文本框中的位置会显示令牌。 您可以使用多个令牌。

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >消息和点按操作在两种平台上看起来都相同。

   仅适用于iOS，选中此复选框可在消息到达时通知应用程序播放声音。 Android会自动播放声音。

   ![](assets/ios-tap-and-notification-hand.png)

   预览另一个平台，然后单击“完成”。

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. 单击&#x200B;**批准并关闭**。

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

恭喜！ 现在，推送通知已准备好发送。

## 深层链接URI {#deep-link-uris}

当订阅者单击推送消息中的按钮时，可将其转到您的应用程序的主页或直接转到应用程序中的特定页面。 深层链接是对应用程序中特定页面的唯一引用，与网站链接非常相似。

深层链接URI由三部分组成：方案名称、路径和标识符。 在以下示例中，“myappname”是方案。 “products”是路径，“purple-shirt”是标识符。 客户点击时，会专门将它们带到应用程序产品页面中的紫色衬衫项目。

![](assets/image2016-7-29-12-3a49-3a1.png)

也就是说，您的应用程序的深层链接结构可能与上述示例不同。 您的开发人员在定义深层链接URI方面有许多选项，因此请要求您的开发人员向您发送您感兴趣使用的页面的URI（链接）。 这将确保您在推送消息中输入的URI指向正确的位置。 开发者可以[在此处查找更多信息](https://developers.marketo.com/mobile/enabling-deep-links-in-your-app/)。

>[!MORELIKETHIS]
>
>* [发送移动推送通知](send-a-mobile-push-notification.md)

>



