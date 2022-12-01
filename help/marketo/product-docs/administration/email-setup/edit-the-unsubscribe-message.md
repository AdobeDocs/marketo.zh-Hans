---
unique-page-id: 2360251
description: 编辑取消订阅消息 — Marketo文档 — 产品文档
title: 编辑退订消息
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# 编辑退订消息 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理员权限**

当您发送营销电子邮件(非[操作](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md))，则取消订阅文本和链接会附加到底部。 您可以更改默认值。 这是方法。

## 在何处进行编辑 {#where-to-make-the-edit}

1. 转到 **管理员** 中。

   ![](assets/edit-the-unsubscribe-message-1.png)

1. 单击 **电子邮件**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除！
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. 编辑 **取消订阅HTML** 和 **取消订阅文本** 单击 **保存更改**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   给你。 _一定要测试！_ 您不希望营销电子邮件中断取消订阅链接。

>[!TIP]
>
>您可以使用 [令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## 默认取消订阅文本 {#default-unsubscribe-text}

如果您需要还原到默认的系统取消订阅，请复制/粘贴以下内容：

取消订阅HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` 取消订阅文本：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[编辑“查看为网页”消息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
