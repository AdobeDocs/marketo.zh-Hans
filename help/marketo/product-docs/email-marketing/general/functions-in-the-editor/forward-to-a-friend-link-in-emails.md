---
unique-page-id: 1900581
description: 在电子邮件中转发到朋友链接 — Marketo文档 — 产品文档
title: 在电子邮件中转发到朋友链接
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# 在电子邮件中转发到朋友链接 {#forward-to-a-friend-link-in-emails}

通过将“转发给朋友”链接添加到电子邮件，您可以跟踪通过此链接收到转发电子邮件的用户，如果数据库中尚不存在这些用户，则自动将其添加为新用户。

例如，假设Keith使用“转发给朋友”链接将电子邮件转发给未知人员Mark。 Mark会自动添加为新人员，并获得他自己的Cookie，他的任何电子邮件和Web活动都会关联到他。 但是，如果Keith在其电子邮件客户端中使用“转发”按钮，则Mark会错误地被编码为Keith，并且其活动会记录为Keith的。

## 添加指向电子邮件模板的链接 {#add-the-link-to-an-email-template}

1. 转到&#x200B;**设计工作室**。

   ![](assets/one-8.png)

1. 查找并选择要为其添加链接的电子邮件模板。 单击&#x200B;**编辑草稿**。

   ![](assets/two-7.png)

1. 将以下HTML代码粘贴到您希望显示“转发给朋友”链接的位置（如果您需要有关此部件的帮助，请咨询您的Web开发人员）：

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >您可以为链接添加样式，使其外观更好看。 例如：
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >不建议在电子邮件模板中使用样式&#x200B;**position：relative**。 这可能会导致“转发给朋友”框的位置和显示出现问题。

1. 单击&#x200B;**预览草稿**，确保模板看起来与您要的一样。

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >请记得批准模板草稿以应用更改。

   现在，使用该模板的所有电子邮件都将具有“转发给朋友”链接。 当电子邮件收件人单击时，将带他们查看电子邮件的Web版本，并显示“转发给朋友”框：

   ![](assets/f2afbox.png)

## 添加指向个人电子邮件的链接 {#add-the-link-to-an-individual-email}

您还可以将“转发给朋友”链接直接添加到电子邮件中。

1. 打开要包含该链接的电子邮件，并在可编辑区域中双击。

   ![](assets/five-4.png)

1. 将光标放在您希望链接出现的位置，然后单击&#x200B;**插入令牌**&#x200B;按钮。

   ![](assets/six-2.png)

1. 选择&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;令牌。

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >此令牌是带有“转发给朋友”框的电子邮件Web版本的URL。

1. 写出您希望链接的显示文本的内容（例如，“转发给朋友”）。

   ![](assets/seven-1.png)

1. 使用Ctrl+X (Windows)或Cmd+X (Mac)剪切&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;令牌。 突出显示“转发给朋友”并单击&#x200B;**插入/编辑链接**&#x200B;按钮。

   ![](assets/eight-1.png)

1. 使用Ctrl/Cmd+V将&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;令牌粘贴到&#x200B;**URL**&#x200B;框中，然后单击&#x200B;**插入**。

   ![](assets/nine.png)

1. 保存编辑并预览新链接！

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >通过接收“转发给朋友”电子邮件添加的新用户默认情况下会取消订阅营销电子邮件。

## 查看转发活动 {#view-forwarding-activity}

您可以在用户的活动日志中查看转发和接收电子邮件的用户。

1. 转到&#x200B;**`Database`**。

   ![](assets/db.png)

1. 双击要查看其活动的用户。

   ![](assets/fourteen.png)

1. 转到&#x200B;**活动日志**&#x200B;选项卡。 双击&#x200B;**已接收转发给好友的电子邮件**&#x200B;或&#x200B;**已转发给好友的电子邮件**&#x200B;以查看详细信息。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**定义**
   >
   >对于已接收的“转发给朋友”电子邮件，人员ID是转发电子邮件的人员。
   >
   >对于“转发给朋友”电子邮件，人员ID是接收电子邮件的人员。

   ![](assets/sixteen.png)

1. 要按ID查看人员，请将&#x200B;**人员ID**&#x200B;复制并粘贴到URL的末尾(上述URL的开头将取决于您的Marketo实例)：

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >我们将在即将到来的修补程序中使&#x200B;**人员ID**&#x200B;可点击并直接链接到该人员。

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >如果接收转发的朋友是未知人员，则会创建一个新人员，其中的“转发给朋友”标记为此人员的&#x200B;**Source**。
   >如果电子邮件是计划的本地资产，则该计划将标记为人员的&#x200B;**客户获取计划**。

## 使用转发活动触发或过滤 {#trigger-or-filter-using-forwarding-activity}

共有六个触发器/过滤器可用于触发流量操作，或按已发送和已接收的“转发给朋友”活动过滤人员。

在智能营销活动的智能列表中，如果您搜索“转发”，则会找到可用的触发器和过滤器。

![](assets/nineteen.png)

## 测试转发给朋友 {#test-forward-to-friend}

要测试“转发给朋友”，请给自己发送一封包含转发链接的电子邮件。 确保通过&#x200B;**发送电子邮件**&#x200B;流程步骤发送，*不是*&#x200B;通过&#x200B;**发送测试电子邮件**。
