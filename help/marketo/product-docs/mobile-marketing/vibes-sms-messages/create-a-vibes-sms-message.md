---
unique-page-id: 11378869
description: 创建访客短信消息 — Marketo文档 — 产品文档
title: 创建访客SMS消息
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 创建访客SMS消息 {#create-a-vibes-sms-message}

以下是如何创建访客短信消息。

>[!AVAILABILITY]
>
>此功能可用作您的Adobe Marketo Engage帐户的加载项。 为了进行正确配置，必须通过Adobe购买。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

>[!NOTE]
>
>短信短信不符合HIPAA标准。

1. 转到 **营销活动** 并右键单击某个项目。

   ![](assets/mobile-right-click-hand.jpg)

1. 单击 **新建本地资产**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >或者，您可以单击 **新建** 下拉菜单。

1. 单击 **SMS消息**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. 输入新短信消息的名称和可选描述，然后单击 **创建**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. 单击 **编辑草稿**.

   ![](assets/edit-draft-hand.jpg)

1. 在消息编辑器中，单击蓝色气泡并开始输入文本。

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >美国和加拿大的限制有所不同，分别为160和130个字符。 如果超过这些字符限制，则可能会拆分消息。 虽然我们会在您超出加拿大限制时显示编辑器，但它已针对美国进行了优化，并根据美国限制拆分消息。

1. 单击 **令牌** 在插入菜单中，向消息中添加令牌。

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >添加令牌可能会导致消息超出字符限制。 然后，该消息将被拆分，从而导致额外费用。

1. 单击 **链接** 在“插入”菜单中添加指向消息的链接。

   ![](assets/full-message-link-hand.jpg)

1. 选择链接类型。 默认“Marketo登录页面”。 如果您选择登陆页面，则需要从下拉列表中选择该登陆页面，然后单击 **插入**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >默认情况下，将选择两个跟踪链接。

1. 如果要改用外部URL，请单击 **外部URL** 按钮，并在URL字段中输入URL。 单击 **插入**.

   ![](assets/insert-link-url-hands.jpg)

1. 该链接将显示在消息中。

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo显示品牌跟踪域的链接预览。 如果清除mkt_tok链接复选框，则链接会更改。 同时清除跟踪链接复选框，URL将缩短为其基本长度(例如，www.mygooglepage.com)。

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >字符数仅反映最低级别消息中包含的字符。

如果插入的内容超过美国的限制，编辑器会将您的消息分成多个部分。 绝对总限制为900个字符。 达到该限制后，在将消息发送到其受众时，该消息将自动被截断。
