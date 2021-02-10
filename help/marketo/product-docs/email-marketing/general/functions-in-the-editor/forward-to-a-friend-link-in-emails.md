---
unique-page-id: 1900581
description: 转发到电子邮件- Marketo Docs —— 产品文档中的好友链接
title: 转发到电子邮件中的朋友链接
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---


# 转发到电子邮件{#forward-to-a-friend-link-in-emails}中的朋友链接

在您的电子邮件中添加“转发到朋友”链接，可跟踪通过此链接收到转发电子邮件的用户，如果他们不在数据库中，还可自动将他们添加为新用户。

例如，假设Keith使用“转发给朋友”链接将电子邮件转发给未知人物Mark。 Mark会自动添加为新人，并被分配自己的Cookie，并且他的任何电子邮件和Web活动都与他关联。 但是，如果Keith使用其电子邮件客户端中的前进按钮，Mark会被错误地调用Keith语音，而他的活动则被记录为Keith&#39;s。

## 添加电子邮件模板{#add-the-link-to-an-email-template}的链接

1. 转到&#x200B;**Design Studio**。

   ![](assets/one-8.png)

1. 查找并选择要添加链接的电子邮件模板。 单击&#x200B;**编辑草稿**。

   ![](assets/two-7.png)

1. 粘贴以下HTML代码，以便显示“转发给朋友”链接（如果您需要有关此部分的帮助，请与Web开发人员协商）:

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >您可以向链接添加样式，使其看起来更好。 例如：
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >我们不建议在电子邮件模板中使用样式&#x200B;**position:relative**。 它可能会导致“转发给朋友”框的位置和显示问题。

1. 单击&#x200B;**预览草稿**&#x200B;以确保模板按您希望的方式显示。

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >请记住批准要应用更改的模板草稿。

   现在，所有使用该模板的电子邮件都将带有“转发给朋友”链接。 当电子邮件收件人单击该按钮时，他们将被带到电子邮件的Web版本，并带有“转发给朋友”框：

   ![](assets/f2afbox.png)

## 将链接添加到单个电子邮件{#add-the-link-to-an-individual-email}

您还可以直接将“转发到朋友”链接添加到电子邮件中。

1. 打开要包含链接的电子邮件，然后在可编辑区域中多次单击。

   ![](assets/five-4.png)

1. 将光标放在希望链接出现的位置，然后单击&#x200B;**插入令牌**&#x200B;按钮。

   ![](assets/six-2.png)

1. 选择&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;令牌。

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >此令牌是带有“转发给朋友”框的Web版电子邮件的URL。

1. 写出您希望链接的显示文本是什么（例如，“转发给朋友”）。

   ![](assets/seven-1.png)

1. 使用Ctrl+X(Windows)或Cmd+X(Mac)剪切&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;标记。 高亮显示“转发给朋友”并单击&#x200B;**插入／编辑链接**&#x200B;按钮。

   ![](assets/eight-1.png)

1. 使用Ctrl/Cmd+V将&#x200B;**`{{system.forwardToFriendLink}}`**&#x200B;标记粘贴到&#x200B;**URL**&#x200B;框中，然后单击&#x200B;**插入**。

   ![](assets/nine.png)

1. 保存编辑并预览新链接！

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >默认情况下，通过收到“转发给朋友”电子邮件而添加的新用户将取消订阅营销电子邮件。

## 视图转发活动{#view-forwarding-activity}

您可以在个人的活动日志中查看转发和接收电子邮件的人。

1. 转到&#x200B;**`Database`**。

   ![](assets/db.png)

1. 多次-单击要视图活动的人。

   ![](assets/fourteen.png)

1. 转到&#x200B;**活动日志**&#x200B;选项卡。 多次-单击&#x200B;**已转发给好友电子邮件**&#x200B;或&#x200B;**已转发给好友电子邮件**&#x200B;以查看详细信息。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**定义**
   >
   >对于“已转发给朋友的电子邮件”，人员ID是转发电子邮件的人。
   >
   >对于“转发给朋友的电子邮件”，人员ID是收到该电子邮件的人。

   ![](assets/sixteen.png)

1. 要按ID视图人员，请将&#x200B;**人员ID**&#x200B;复制并粘贴到URL的末尾（该URL的开头取决于您的Marketo实例）:

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >我们将使&#x200B;**人员ID**&#x200B;变为可点击状态并直接链接到即将发布的修补程序中的人员。

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >如果接收转发的朋友是未知的人，则会创建一个新人，其“转发给朋友”标记为该人的&#x200B;**源**。
   >如果电子邮件是项目的本地资产，则项目将标记为人员的&#x200B;**客户获取项目**。

## 使用转发活动{#trigger-or-filter-using-forwarding-activity}的触发器或过滤器

您可以使用六个触发器/过滤器触发流动操作或通过发送和接收的“转发给朋友”活动过滤人员。

在智能活动的智能列表中，如果搜索“转发”，您将找到可用的触发器和过滤器。

![](assets/nineteen.png)

## 测试转发给朋友{#test-forward-to-friend}

要测试“转发给朋友”，请通过转发链接给自己发送电子邮件。 确保通过&#x200B;**发送电子邮件**&#x200B;流程步骤&#x200B;*不*&#x200B;通过&#x200B;**发送测试电子邮件**&#x200B;发送。
