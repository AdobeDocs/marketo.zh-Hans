---
unique-page-id: 2360253
description: 自定义管理员电子邮件中的以网页形式查看链接文本和HTML ，同时保持所需变量不变。
title: 编辑“以网页形式查看”消息
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
TQID: https://experienceleague.adobe.com/mREJHheKv7c16atJ17pv8S9ZGUoLnD8jd5jyk6QtgR8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 153
ht-degree: 31%

---

# 编辑“以网页形式查看”消息 {#edit-the-view-as-web-page-message}

了解如何编辑“[以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)”文本。

>[!NOTE]
>
>**需要管理员权限**

## 编辑“以网页形式查看”消息 {#edit-the-view-as-web-page-message-1}

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除它们！
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >第二部分`##MKT_TOK##`是该人员的[!UICONTROL Munchkin] Cookie。 这样可以确保在用户单击链接时对其进行适当跟踪。

1. 编辑您喜欢的&#x200B;**[!UICONTROL View as Web Page HTML]**&#x200B;和&#x200B;**[!UICONTROL View as Web Page Text]**&#x200B;版本，然后单击&#x200B;**[!UICONTROL Save Changes]**。

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>请务必避免：
>
>* 向任一HTML框添加其他URL
>* 在文本版本中置入HTML

发送测试电子邮件以验证格式。

## 默认“以网页形式查看”文本 {#default-view-as-web-page-text}

如果您需要还原到默认系统“[!UICONTROL View as Web Page]”，请复制/粘贴以下内容：

**[!UICONTROL View as Web Page HTML]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL View as Web Page Text]**:

要以网页的形式查看此电子邮件，请转到以下地址：
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
