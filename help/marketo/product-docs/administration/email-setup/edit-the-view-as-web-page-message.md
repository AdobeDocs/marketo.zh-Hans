---
unique-page-id: 2360253
description: 编辑“查看网页”消息 — Marketo文档 — 产品文档
title: 编辑“查看为网页”消息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 编辑“查看为网页”消息 {#edit-the-view-as-web-page-message}

如果需要编辑[作为网页查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)“ text，这是方法。

>[!NOTE]
>
>**需要管理员权限**

## 编辑“查看为网页”消息 {#edit-the-view-as-web-page-message-1}

1. 转到 **管理员** 的上界。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 单击 **电子邮件**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分 `##MKT_TOK##` 是那个人的Munchkin Cookie。 它可确保用户在单击链接时获得适当的Cookie。

1. 编辑 **查看为网页HTML** 和 **查看为网页文本** 单击 **保存更改**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>请务必避免：
>
>* 向任一HTML框添加其他URL
>* 在文本版本中置入HTML


给你。 发送测试电子邮件以确保格式化。

## 默认的“查看网页”文本 {#default-view-as-web-page-text}

如果您需要还原到默认的系统“查看为网页”，请复制/粘贴以下内容：

**查看为网页HTML:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**查看为网页文本：**

要以网页形式查看此电子邮件，请转到以下地址：
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

就这样！
