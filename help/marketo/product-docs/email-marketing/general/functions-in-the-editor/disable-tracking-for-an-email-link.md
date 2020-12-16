---
unique-page-id: 1900579
description: 禁用电子邮件链接的跟踪- Marketo Docs —— 产品文档
title: 禁用电子邮件链接的跟踪
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# 禁用电子邮件链接的跟踪 {#disable-tracking-for-an-email-link}

有时，您不希望对电子邮件中 **的链接启用** “营销人员跟踪URL”。 当目标页面不支持URL参数并可能导致链接断开时，此功能很有用。

1. 选择您的电子邮件，然后单 **击“编****辑草稿**”。

   ![](assets/one-7.png)

1. 多次-单击包含链接的可编辑部分。

   ![](assets/two-6.png)

1. 单击相关链接，然后单击“插入/ **编辑链接** ”按钮。

   ![](assets/three-6.png)

1. 在“编辑链接”弹出窗口中，取消选中“ **跟踪链接** ”复选框。

   ![](assets/four-4.png)

1. 您会注意到“包 **括mkt_tok”框消失** 。 单击“ **应用**”。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >仅取消 **选中“包括mkt** _tok”仍允许跟踪链接，但重定向后，目标URL将不包括mkt_tok查询字符串参数。 此参数由Marketo登陆页和Munchkin使用，以确保对个人活动进行正确跟踪（如当某人取消订阅电子邮件时）。 除非由于参数存在，您在网站上看到异常行为，否则应避免使用此功能。

1. 单击 **保存**。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >是否要禁用电子邮件模板中链接的点击跟 **踪**? 使用以下格式：
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >如果您需要实施此功能的帮助，请咨询您的Web开发人员。

不错！ 您现在已禁用链接的跟踪。
