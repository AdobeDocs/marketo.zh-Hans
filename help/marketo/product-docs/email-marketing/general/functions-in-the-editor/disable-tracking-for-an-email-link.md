---
unique-page-id: 1900579
description: 禁用电子邮件链接的跟踪 — Marketo文档 — 产品文档
title: 禁用电子邮件链接的跟踪
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# 禁用电子邮件链接的跟踪 {#disable-tracking-for-an-email-link}

有时，您不想启用 **Marketo跟踪URL** 电子邮件中的链接。 当目标页面不支持URL参数并可能导致链接断开时，此操作非常有用。

1. 选择您的电子邮件并单击 **编辑草稿**.

   ![](assets/one-7.png)

1. 双击包含该链接的可编辑部分。

   ![](assets/two-6.png)

1. 单击相关链接，然后单击 **插入/编辑链接** 按钮。

   ![](assets/three-6.png)

1. 在“编辑链接”弹出窗口中，取消选中 **跟踪链接** 复选框。

   ![](assets/four-4.png)

1. 你会注意到 **包含mkt_tok框** 消失。 单击 **应用**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >正在取消检查 **包括mkt_tok** 仍将允许跟踪该链接，但重定向后，目标URL将不包含mkt_tok查询字符串参数。 Marketo登陆页面和Munchkin会使用此参数来确保正确跟踪人员活动（例如，人员取消订阅电子邮件时）。 您应避免使用此功能，除非由于参数存在，您在网站上看到异常行为。

1. 单击 **保存**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >想要禁用电子邮件中链接的点击跟踪 **模板**? 使用以下格式：
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >如果您在实施此功能时需要帮助，请咨询Web开发人员。

不错！ 您现在已禁用链接的跟踪。
