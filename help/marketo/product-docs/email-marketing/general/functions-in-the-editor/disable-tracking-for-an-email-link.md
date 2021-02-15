---
unique-page-id: 1900579
description: 禁用电子邮件链接的跟踪 — Marketo Docs — 产品文档
title: 禁用电子邮件链接的跟踪
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# 禁用电子邮件链接{#disable-tracking-for-an-email-link}的跟踪

有时，您不希望对电子邮件中的链接启用&#x200B;**Marketo跟踪URL**。 当目标页面不支持URL参数并可能导致链接断开时，此功能非常有用。

1. 选择您的电子邮件，然后单击&#x200B;**编辑草稿**。

   ![](assets/one-7.png)

1. 多次单击包含该链接的可编辑部分。

   ![](assets/two-6.png)

1. 单击相关链接，然后单击&#x200B;**插入/编辑链接**&#x200B;按钮。

   ![](assets/three-6.png)

1. 在“编辑链接”弹出窗口中，取消选中&#x200B;**“跟踪链接**”复选框。

   ![](assets/four-4.png)

1. 您会注意到&#x200B;**Include mkt_tok box**&#x200B;消失。 单击&#x200B;**应用**。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >仅取消检查&#x200B;**“包括mkttok**”仍允许跟踪链接，但在重定向后，目标URL将不包括mkttok查询字符串参数。 此参数由Marketo登陆页和Munchkin使用，以确保对个人活动进行正确跟踪（如当某人从电子邮件中取消订阅时）。 您应避免使用此功能，除非由于参数存在，您在网站上看到异常行为。

1. 单击&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >是否要禁用电子邮件&#x200B;**template**中链接的点击跟踪？ 使用以下格式：
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >如果您需要实施此解决方案的帮助，请咨询您的Web开发人员。

不错！ 您现在已禁用链接的跟踪。
