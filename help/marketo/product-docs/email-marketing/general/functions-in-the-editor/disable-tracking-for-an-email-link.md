---
unique-page-id: 1900579
description: 禁用电子邮件链接的跟踪 — Marketo文档 — 产品文档
title: 禁用电子邮件链接跟踪
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 5%

---

# 禁用电子邮件链接跟踪 {#disable-tracking-for-an-email-link}

有时，您不希望通过电子邮件在链接上启用&#x200B;**Marketo跟踪URL**。 当目标页面不支持URL参数并且可能导致链接断开时，这将很有用。

此外，如果电子邮件是在&#x200B;**和** 365天之前发送的，且过去180天内无人单击任何链接，则Marketo Engage会从我们的数据库中修剪指向URL的路由，这会导致链接断开。 因此，如果您需要永久性链接，则应当禁用跟踪。

1. 选择您的电子邮件并单击&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/one-7.png)

1. 双击包含链接的可编辑部分。

   ![](assets/two-6.png)

1. 单击有问题的链接，然后单击&#x200B;**插入/编辑链接**&#x200B;按钮。

   ![](assets/three-6.png)

1. 在编辑链接弹出窗口中，取消选中&#x200B;**[!UICONTROL Track Link]**&#x200B;复选框。

   ![](assets/four-4.png)

1. 您会注意到&#x200B;**[!UICONTROL Include mkt_tok]框**&#x200B;消失。 单击 **[!UICONTROL Apply]**。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >仅取消选中&#x200B;**包含mkt_tok**&#x200B;仍允许跟踪链接，但在重定向后，目标URL将不包含mkt_tok查询字符串参数。 此参数供Marketo登陆页面和Munchkin使用，以确保正确跟踪人员活动（例如，当人员取消订阅电子邮件时）。 您应该避免使用此功能，除非您因参数存在而在网站上看到奇怪的行为。

1. 单击 **[!UICONTROL Save]**。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >如果要禁用电子邮件模板中链接或电子邮件的[文本版本](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"}的点击跟踪，请在字符串的`mktNoTrack`开头&#x200B;*处添加*，而不是在结尾处添加，如以下示例所示：`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`。 否则，可能会导致链接消失。 如果您需要有关实施上述代码的帮助，请咨询您的Web开发人员。
