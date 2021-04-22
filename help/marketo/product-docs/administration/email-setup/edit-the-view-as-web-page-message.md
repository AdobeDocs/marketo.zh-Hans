---
unique-page-id: 2360253
description: 编辑“视图为网页”消息 — Marketo Docs — 产品文档
title: 编辑“视图为网页”消息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# 编辑“视图为网页”消息{#edit-the-view-as-web-page-message}

如果您需要将“[视图作为Webpage](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)”文本进行编辑，请按照以下说明操作。

>[!NOTE]
>
>**需要管理权限**

## 编辑“视图为网页”消息{#edit-the-view-as-web-page-message-1}

1. 在&#x200B;**Admin**&#x200B;下，单击&#x200B;**电子邮件**。

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除它们！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分`##MKT_TOK##`是该人的Munchkin Cookie。 它确保用户在单击链接时获得适当的Cookie。

1. 根据您的喜好将&#x200B;**视图编辑为网页HTML**&#x200B;和&#x200B;**视图为网页文本**&#x200B;版本，然后单击&#x200B;**保存更改**。

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>务必避免：
>
>* 向任一HTML框添加其他URL
>* 将HTML置入文本版本


给你。 发送测试电子邮件以确保格式。

## 默认“视图为网页”文本{#default-view-as-web-page-text}

如果您曾经需要还原到默认系统“视图为网页”，请复制/粘贴以下内容：

**视图为网页HTML:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**视图为网页文本：**

要将此电子邮件视图为网页，请转到以下地址：
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`砰！ 你完了。
