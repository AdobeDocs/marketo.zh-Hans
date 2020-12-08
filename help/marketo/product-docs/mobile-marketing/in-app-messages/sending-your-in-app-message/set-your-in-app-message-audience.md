---
unique-page-id: 10617431
description: 设置应用程序内消息受众- Marketo Docs —— 产品文档
title: 设置应用程序内消息受众
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 设置应用程序内消息受众 {#set-your-in-app-message-audience}

第一步是决定谁应接收您的应用程序内消息。 您需要设置智能列表。

1. 单击 **编辑智能列表**。

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. 在智能列表中，将自动填充“具有移动应用程序”活动触发器。 单击下拉框并选择要将消息放入的应用程序。

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >当前不支持应用程序内消息项目的“移动应用程序”字段的多个值。

1. **App Open** 是默认的“操作”设置，但您可以选择已设置的任何自定义事件。

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >默认触发器（应用程序打开）和开发人员添加到代码的任何自定义触发器将自动显示在“操作”选择器中。 如果缺少自定义事件，请咨询您的开发人员，确保他们已将自定义事件添加到应用程序。 请注意，自定义事件编码和批准过程可能需要一些时间才能完成。 请参 [阅本文](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md) ，了解详细信息。

1. 约束可用于“具有 **移动应用程序活动** ”触发器（如果需要）。

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. 您可以向智能列表添加过滤器，以限制接收您的应用程序内消息的用户。 在此示例中，使用“ **客户获取日期** ”过滤器，将只发送2016年6月9日获取的人员应用程序内消息。

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. 返回至您的应用程序内消息控制面板。 在下拉列表中设置显示限制。

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >默认显示限制为“每 **个会话一次”**。 如果希望消息在收件人响应后停止显示，请选择“ **每次直到点击**”。 如果它应该每次显示，无论收件人做什么，请 **每次选择**。

   ![](assets/image2016-5-9-15-3a32-3a6.png)

干得好！ 你有受众套。 你赢得了蓝条和绿勾号。

选择应 [用程序内消息的时间](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)!
