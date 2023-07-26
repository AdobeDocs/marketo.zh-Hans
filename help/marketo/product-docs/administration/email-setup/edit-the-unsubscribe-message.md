---
unique-page-id: 2360251
description: 编辑取消订阅消息 — Marketo文档 — 产品文档
title: 编辑取消订阅消息
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# 编辑取消订阅消息 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理员权限**

当您发送营销电子邮件时(非[可操作](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md))，取消订阅文本和链接将附加到底部。 您可以更改默认值。 具体方法如下。

## 进行编辑的位置 {#where-to-make-the-edit}

1. 转到 **[!UICONTROL 管理员]** 部分。

   ![](assets/edit-the-unsubscribe-message-1.png)

1. 单击 **[!UICONTROL 电子邮件]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除它们！
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. 编辑 **[!UICONTROL 取消订阅HTML]** 和 **[!UICONTROL 取消订阅文本]** 您喜欢的版本，然后单击 **[!UICONTROL 保存更改]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   给你。 _务必进行测试！_ 您不希望营销电子邮件具有中断的取消订阅链接。

>[!TIP]
>
>您可以使用自定义取消订阅HTML在电子邮件中的位置 [令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## 默认取消订阅文本 {#default-unsubscribe-text}

如果您需要恢复为默认系统取消订阅，请复制/粘贴以下内容：

[!UICONTROL 取消订阅HTML]：
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` [!UICONTROL 取消订阅文本]：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[编辑“以网页形式查看”消息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
