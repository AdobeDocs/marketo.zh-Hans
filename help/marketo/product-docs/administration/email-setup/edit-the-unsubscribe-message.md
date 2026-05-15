---
unique-page-id: 2360251
description: 更改管理员电子邮件中附加到营销电子邮件的默认取消订阅文本和链接。
title: 编辑取消订阅消息
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
TQID: https://experienceleague.adobe.com/2wAcUvsELVvNhk0HpdNdkWJLopFn3IC4X-lUSQlCs5Q
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 128
ht-degree: 9%

---

# 编辑取消订阅消息 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**需要管理员权限**

当您发送营销电子邮件（非[可操作的](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)）时，取消订阅文本和链接将附加到底部。 您可以更改默认值。

## 进行编辑的位置 {#where-to-make-the-edit}

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;部分。

   ![](assets/edit-the-unsubscribe-message-1.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >以下变量至关重要。 不要删除它们！
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. 编辑您喜欢的&#x200B;**[!UICONTROL Unsubscribe HTML]**&#x200B;和&#x200B;**[!UICONTROL Unsubscribe Text]**&#x200B;版本，然后单击&#x200B;**[!UICONTROL Save Changes]**。

   ![](assets/edit-the-unsubscribe-message-3.png)

>[!TIP]
>
>* 记得测试。 您不希望营销电子邮件具有中断的取消订阅链接。
>
>* 您可以使用[令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)自定义取消订阅HTML在电子邮件中的位置。

## 默认取消订阅文本 {#default-unsubscribe-text}

如果您需要恢复为默认系统取消订阅消息，请复制/粘贴以下内容：

[!UICONTROL Unsubscribe HTML]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>`
<br>
[!UICONTROL Unsubscribe Text]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[编辑“以网页形式查看”消息](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
