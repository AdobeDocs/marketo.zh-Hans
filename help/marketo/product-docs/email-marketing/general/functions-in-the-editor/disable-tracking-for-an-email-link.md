---
unique-page-id: 1900579
description: 禁用电子邮件链接的跟踪 — Marketo文档 — 产品文档
title: 禁用电子邮件链接的跟踪
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# 禁用电子邮件链接的跟踪 {#disable-tracking-for-an-email-link}

有时，您不希望通过电子邮件在链接上启用&#x200B;**Marketo跟踪URL**。 当目标页面不支持URL参数并且可能导致链接断开时，这将很有用。

1. 选择您的电子邮件并单击&#x200B;**编辑草稿**。

   ![](assets/one-7.png)

1. 双击包含链接的可编辑部分。

   ![](assets/two-6.png)

1. 单击有问题的链接，然后单击&#x200B;**插入/编辑链接**&#x200B;按钮。

   ![](assets/three-6.png)

1. 在编辑链接弹出窗口中，取消选中&#x200B;**跟踪链接**&#x200B;复选框。

   ![](assets/four-4.png)

1. 您会注意到&#x200B;**包含mkt_tok框**&#x200B;已消失。 单击&#x200B;**应用**。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >仅取消选中&#x200B;**包含mkt_tok**&#x200B;仍允许跟踪链接，但在重定向后，目标URL将不包含mkt_tok查询字符串参数。 此参数由Marketo登录页面和Munchkin使用，以确保正确跟踪人员活动（例如，当人员取消订阅电子邮件时）。 您应该避免使用此功能，除非您因参数存在而在网站上看到奇怪的行为。

1. 单击&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >想要禁用电子邮件&#x200B;**模板**中链接的点击跟踪？ 使用此格式：
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >如果您需要实施此功能的帮助，请咨询您的Web开发人员。

太好了！ 您现在已禁用对链接的跟踪。
