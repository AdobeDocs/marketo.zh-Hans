---
unique-page-id: 4720758
description: 发行说明 — 2015年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2015年1月
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 发行说明：2015年1月 {#release-notes-january}

2015年1月版本中包含以下功能。 请检查您的Marketo版本是否提供了相关功能。 发布后，请务必返回以查找指向每个功能的详细文章的链接！

## 营销自动化更新 {#marketing-automation-updates}

**便于移动使用的登陆页面**

您现在可以 [为登陆页面构建移动视图](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) 从登陆页面编辑器中。 无论使用什么设备，您都可以有效地传递您的消息，并通过定制内容以方便移动使用，从而提高参与度。 此功能将在版本发布后的一周内逐步推出。

[ — 登陆页面演练视频 — ](https://youtu.be/aPQHlG2X6c0)

**新的Rest API调用**

Lead &amp; Activity ReST API的三个新调用：

* 删除潜在客户
* 按项目ID获取潜在客户
* 获取已删除的潜在客户

此外，还有一个适用于同步潜在客户的新选项，即异步写入潜在客户更改以实现更快的API调用。 完整详细信息将在发布后提供，网址为 [developers.marketo.com](https://developers.marketo.com)

**电子邮件脚本自定义对象支持**

现在，可从电子邮件脚本中访问与帐户对象关联的自定义对象！

## 实时个性化 {#real-time-personalization}

**Google和Facebook的个性化再营销**

再营销可向访问过您网站的人显示广告。 您现在可以在以下位置个性化再营销活动： [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) 和 [facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) 使用来自实时个性化的数据。 向来自不同行业的受众、指定帐户列表、公司规模或任何已知潜在客户的数据进行再营销。

[指定帐户列表模块](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

对指定帐户模块的增强将提高用户的匹配率和验证。 新增项目包括：

* 使用Lead的电子邮件地址从指定帐户列表中匹配组织（也适用于仅RTP客户）
* 支持每个帐户最多10万条记录
* 要查看和下载的CSV文件模板

![](assets/image2015-1-14-11-3a12-3a16.png)

**更新了RTP标记选项**

“帐户设置”下的“RTP标记”选项已更新为包括：

1. CDN和异步（推荐的标记）
1. CDN和同步（高速）
1. 不带CDN的异步标记
1. 不带CDN的同步标记

为获得最佳性能，建议将标记放在网页中标题的顶部，之后 `<head>`. 所有标记均允许使用 [RTP API](https://developers.marketo.com/documentation/websites/rtp-js-api/). 有关如何部署RTP标记的信息，请参阅 [此处](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
