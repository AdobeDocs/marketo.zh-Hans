---
unique-page-id: 2360253
description: 编辑“以网页形式查看”消息 — Marketo文档 — 产品文档
title: 编辑“以网页形式查看”消息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 编辑“以网页形式查看”消息 {#edit-the-view-as-web-page-message}

如果您需要编辑&quot;[以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)“文本，下面是操作方法。

>[!NOTE]
>
>**需要管理员权限**

## 编辑“以网页形式查看”消息 {#edit-the-view-as-web-page-message-1}

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 单击 **[!UICONTROL 电子邮件]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除它们！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分 `##MKT_TOK##` 是 [!UICONTROL munchkin] 该人员的Cookie。 它确保访客在单击链接时被正确编码。

1. 编辑 **[!UICONTROL 以网页HTML查看]** 和 **[!UICONTROL 以网页文本查看]** 版本和单击时显示的内容 **[!UICONTROL 保存更改]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>请务必避免：
>
>* 向任一HTML框添加其他URL
>* 在文本版本中置入HTML


给你。 发送测试电子邮件以确保格式化。

## 默认“以网页形式查看”文本 {#default-view-as-web-page-text}

如果您需要还原到默认系统”[!UICONTROL 以网页查看]“”，复制/粘贴以下内容：

**[!UICONTROL 以网页HTML查看]**：

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL 以网页文本查看]**：

要以网页形式查看此电子邮件，请转到以下地址：
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

就是这样！
