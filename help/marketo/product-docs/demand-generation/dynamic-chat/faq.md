---
description: Dynamic Chat常见问题解答 — Marketo文档 — 产品文档
title: Dynamic Chat常见问题解答
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: ed833219e5074ae646e07db599e7da50665c453b
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Dynamic Chat常见问题解答 {#dynamic-chat-faq}

请参阅以下内容，了解有关Dynamic Chat的一些常见问题的答案。

**我似乎无权访问Dynamic Chat。 如何获取？**

请联系您的Marketo Engage管理员，确保他们已[将您添加为Adobe Admin Console中的用户](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"}。

**我是否可以在公司网站上的任何位置安装Dynamic Chat，或者它是否只能在Marketo登录页中使用？**

Dynamic ChatJavaScript代码片段可以安装在任何网站以及Marketo登陆页面上。

**数据存储用于报告的时间有多长？**

90天。 有关限制/参数的完整列表，请访问Marketo Engage[产品描述页](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}。

**Dynamic Chat是否支持英语以外的任何语言？**

可以。Dynamic Chat支持以下语言：法语、西班牙语、德语、日语、荷兰语、意大利语、巴西葡萄牙语、朝鲜语、简体中文和繁体中文。 请参阅[更改语言](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}以了解详情。

**是否支持AI/NLP功能？**

我们不支持AI/NLP功能。

**如何定位匿名用户？**

在对话框中，您需要使用&#x200B;_人员电子邮件为空_&#x200B;属性。

**什么符合参与对话的条件？**

一旦访客对对话框或对话流中的机器人做出响应，就会发生参与的对话。 如果访客打开了聊天机器人但未响应机器人（例如，选择响应或提交信息），则不会计为参与。

**如果达到每月参与会话数上限，会发生什么情况？**

当您达到每月参与对话限制时，所有发布的对话框和对话流将停止触发，直到您提高限制或在下个月初重置限制为止。

**我如何知道何时接近参与会话上限？**

当您达到90%的参与对话限制时，Dynamic Chat管理员将收到电子邮件通知，所有用户都将看到Dynamic Chat中的横幅通知。

**如果访客参与对话，然后又与实时代理连接，那么这是否计为一次参与还是两次参与？**

对于Select程序包上的客户，这将计为两个单独的参与 — 一个用于Dialogue参与，另一个用于实时聊天参与。 对于Prime程序包上的客户，实时聊天参与次数不单独计数，因此这仅计为一次参与。

**参与对话限制重置的频率是多少？**

在每个日历月的第一天重置参与的对话限制。

**聊天机器人为何不在我完成对话后返回？**

对话框设计为仅向访客显示一次。 因此，一旦访客到达对话框中的任何给定分支的结尾，该对话框即被视为完成，不会再向该访客显示。

**当我单击“我的Marketo”中的“Dynamic Chat”图标并登录到Adobe Experience Cloud时，为什么会收到以下消息？ _您的Adobe ID似乎未与Adobe Experience Cloud解决方案帐户关联_。“**”

这很可能表明您尚未在Adobe Admin Console中添加为Dynamic Chat用户。 请联系您Adobe组织的系统管理员或产品管理员，以获取Dynamic Chat以请求访问Dynamic Chat的权限。

**如何访问参与对话的记录？**

任何已知潜在客户均可以通过Marketo Engage中的“参与对话”活动参与Dynamic Chat对话，其Dynamic Chat状态为“已完成”或“已丢弃”。

**访客参与对话后，是否可以重新开始对话或返回上一个问题？**

目前没有系统化的方法重新开始对话或返回上一点，但这在Dynamic Chat路线图上。

**Dynamic Chat是否与Salesforce集成？**

Dynamic Chat通过Marketo EngageSalesforce集成与Salesforce集成。

**我的日历已连接至Dynamic Chat，并且我包含在路由规则中，为什么我没有收到任何会议？**

这最可能表明您的日历连接需要重新进行身份验证。 更改日历提供商的密码时，最常出现这种情况，并且Dynamic Chat断开连接。 您只需转到Dynamic Chat中的“代理设置”页面，然后单击“重新验证日历”即可。

**对话与对话流之间有何区别？**

对话框是一种自动向符合一组已定义的定位标准的Web访客显示的对话。 对话流仅显示在Web上执行特定操作（如按按钮）的访客中。

**是否可以使用Dynamic Chat直接从电子邮件预订会议？**

是！[了解如何操作](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}。

**“已参与”或“已获得人员”等术语的含义是什么？**

Dynamic Chat中使用多个术语。 其中许多的定义可在各自区域的帮助文章中找到。

* 可以在此处[&#128279;](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}找到“已获得人员”等Analytics术语。
* 可以在此处[&#128279;](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}找到智能列表触发器/筛选器定义。
* 各种流Designer卡片[的说明可在此处](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}找到。

**我是否可以在没有Marketo Engage的情况下使用Dynamic Chat？**

不会。虽然Dynamic Chat是独立于Marketo Engage的应用程序，但两者之间有着密不可分的联系。
