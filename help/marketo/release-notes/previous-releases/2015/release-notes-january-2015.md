---
unique-page-id: 4720758
description: 发行说明 — 2015年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2015年1月
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 发行说明：2015年1月 {#release-notes-january}

2015年1月版中包含以下功能。 请查看您的Marketo版以了解功能的可用情况。 发布后，请务必回访以查找每个功能的详细文章链接！

## 营销自动化更新 {#marketing-automation-updates}

**移动设备友好登陆页面**

您现在可以 [构建登陆页面的移动视图](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) 从登陆页面编辑器中。 无论使用何种设备，都可以有效地传递消息，并通过定制内容以便在移动中轻松使用来提高参与度。 此功能将在发布后的一周内逐步推出。

[ — 登陆页面演练视频 — ](https://youtu.be/aPQHlG2X6c0)

**新的Rest API调用**

对潜在客户和活动ReST API的三个新调用：

* 删除潜在客户
* 按项目ID获取潜在客户
* 获取已删除的潜在客户

此外，还为同步潜在客户提供了一个新选项，用于异步写入潜在客户更改，以加快API调用速度。 完整的详细信息将在以下位置发布之后提供： [developers.marketo.com](https://developers.marketo.com)

**电子邮件脚本自定义对象支持**

现在，从电子邮件脚本中访问与帐户对象关联的自定义对象！

## 实时个性化 {#real-time-personalization}

**针对Google和Facebook的个性化再营销**

再营销可向访问过您网站的用户显示广告。 您现在可以在 [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) 和 [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) 使用来自实时个性化的数据。 向来自不同行业的受众、指定的帐户列表、公司规模或任何已知潜在客户的数据进行再营销。

[指定帐户列表模块](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

增强了“指定帐户”模块，将提高用户的匹配率和验证率。 新增内容包括：

* 使用潜在客户的电子邮件地址匹配您的指定帐户列表中的组织（也适用于仅限RTP的客户）
* 支持每个帐户最多10万条记录
* 用于查看和下载的CSV文件模板

![](assets/image2015-1-14-11-3a12-3a16.png)

**更新了RTP标记选项**

更新了“帐户设置”下的RTP标记选项以包含：

1. CDN和异步（推荐的标记）
1. CDN和同步（高速）
1. 无CDN的异步标记
1. 无CDN的同步标记

为获得最佳性能，建议在 `<head>`. 所有标记均允许使用 [RTP API](https://developers.marketo.com/documentation/websites/rtp-js-api/). 有关如何部署RTP标记的信息，请参阅 [此处](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
