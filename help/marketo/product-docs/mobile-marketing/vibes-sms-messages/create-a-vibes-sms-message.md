---
unique-page-id: 11378869
description: 创建Vibes SMS消息 — Marketo Docs — 产品文档
title: 创建浏览SMS消息
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# 创建查看SMS消息{#create-a-vibes-sms-message}

下面介绍如何创建Vibes SMS消息。

1. 转到&#x200B;**营销活动**&#x200B;并右键单击项目。

   ![](assets/mobile-right-click-hand.jpg)

1. 单击&#x200B;**新建本地资产**。

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >或者，也可以单击&#x200B;**新建**&#x200B;下拉列表。

1. 单击&#x200B;**SMS Message**。

   ![](assets/new-local-asset-selection-hand.jpg)

1. 输入新SMS消息的名称和可选说明，然后单击&#x200B;**创建**。

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. 单击&#x200B;**编辑草稿**。

   ![](assets/edit-draft-hand.jpg)

1. 在消息编辑器中，在蓝色气泡内单击并开始输入文本。

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >美国和加拿大的限制不同，分别为160和130个字符。 如果超出这些字符限制，则可能会拆分您的消息。 当我们显示您何时超出加拿大限制时，该编辑器已针对美国进行优化，并根据美国限制拆分消息。

1. 单击“插入”菜单中的&#x200B;**令牌**，向消息中添加令牌。

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >添加令牌可能导致消息超出字符限制。 然后，消息将拆分，导致额外费用。

1. 单击“插入”菜单中的&#x200B;**链接**，添加指向消息的链接。

   ![](assets/full-message-link-hand.jpg)

1. 选择链接类型。 默认为Marketo登陆页。 如果执行此操作，您需要从下拉菜单中选择登陆页，然后单击&#x200B;**插入**。

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >默认情况下，将选择两个跟踪链接。

1. 如果要改用外部URL，请单击&#x200B;**外部URL**&#x200B;按钮，并在URL字段中输入URL。 单击&#x200B;**插入**。

   ![](assets/insert-link-url-hands.jpg)

1. 消息中将显示该链接。

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo显示品牌跟踪域的链接预览。 如果清除mkt_tok链接复选框，则链接会更改。 同时清除“跟踪链接”复选框，URL将缩短到其基本长度(例如，www.mygooglepage.com)。

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >字符计数只反映最低消息中包含的字符。

如果插入的内容超过美国的限制，编辑器会将您的消息分为多个部分。 绝对总限制为900个字符。 达到该限制后，消息将在发送到其受众时自动截断。
