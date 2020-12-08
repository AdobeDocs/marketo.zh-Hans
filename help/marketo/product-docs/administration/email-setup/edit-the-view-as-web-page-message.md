---
unique-page-id: 2360253
description: 编辑“视图为网页”消息- Marketo Docs —— 产品文档
title: 编辑“视图为网页”消息
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# 编辑“视图为网页”消息 {#edit-the-view-as-web-page-message}

如果您需要编辑“ [视图作为网页](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)”文本，请查看方法。

>[!NOTE]
>
>**需要管理员权限**

## 编辑“视图为网页”消息 {#edit-the-view-as-web-page-message-1}

1. 在“管 **理员**”下，单 **击“电子邮件**”。

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除它们！
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK##
   >    
   >    
   >第二部分##MKT_TOK##是该人的Munchkin cookie。 它确保用户在单击链接时获得适当的Cookie。

1. 根据 **您的喜好，将视图编辑** 为网页HTML和**视图编辑为网页文本**版本，然后单击 **保存更改**。

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>请务必避免：
>
>* 向任一HTML框添加其他URL
>* 将HTML置入文本版本

>



给你。 发送测试电子邮件以确保格式化。

## 默认“视图为网页”文本 {#default-view-as-web-page-text}

如果您曾经需要还原到默认系统“视图为网页”，请复制／粘贴以下内容：

**视图为网页HTML:**`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **视图为网页文本：**

要将此电子邮件视图为网页，请转到以下地址：`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` 砰！ 你完了。
