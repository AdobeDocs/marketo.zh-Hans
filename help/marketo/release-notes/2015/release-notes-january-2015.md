---
unique-page-id: 4720758
description: 发行说明- 2015年1月- Marketo Docs —— 产品文档
title: 发行说明- 2015年1月
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# 发行说明：2015年1月 {#release-notes-january}

2015年1月版包含以下功能。 请查看您的Marketo Edition以了解功能可用性。 发布后，请务必回来查找每个功能的详细文章的链接！

## 营销自动化更新 {#marketing-automation-updates}

**Rick DeCosta的新照片！**

Rick是SmartBear的Marketo客户，拥有令人难以置信 [的照片集](https://www.flickr.com/photos/rickdecosta)。 看看他们！

## 移动友好登陆页 {#mobile-friendly-landing-pages}

您现在可以 [从视图编辑器中为登陆页](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) 构建移动登陆页。 无论使用何种设备，都能高效地传达您的信息，并通过定制内容来随时随地轻松消费来提高参与度。 此功能将在发布后的一周内逐步推出。

`<iframe width="420" height="315" src="//www.youtube-nocookie.com/embed/aPQHlG2X6c0" frameborder="0" allowfullscreen></iframe>`

**新的ReST API调用**

对潜在客户和活动ReST API的三次新调用：

* 删除潜在客户
* 按项目ID获取潜在客户
* 获取已删除的潜在客户

此外，还有一个新的“同步潜在客户”选项，用于异步编写潜在客户更改以进行更快的API调用。 发布后，将在developers.marketo.com上 [获得完整的详细信息](http://developers.marketo.com)

**电子邮件脚本自定义对象支持**

现在从电子邮件脚本中访问与帐户对象关联的自定义对象！

## 实时个性化 {#real-time-personalization}

**Google和Facebook的个性化再营销**

再营销向访问过您网站的用户显示广告。 您现在可以使用实时个 [性化](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)[数据在](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) Google和Facebook上个性化您的再营销活动。 向来自不同行业的受众、指定帐户列表、公司规模或任何已知潜在客户的数据进行再营销。

[指定帐户列表模块](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

对“指定帐户”模块的增强将提高用户的匹配率和验证率。 新增包括：

* 使用潜在客户的电子邮件地址与指定帐户列表中的组织匹配（也适用于仅限RTP的客户）
* 支持每个帐户最多10万条记录
* 视图和下载CSV文件模板

![](assets/image2015-1-14-11-3a12-3a16.png)

更新的RTP标签选项

[“Account](http://docs.marketo.com/display/docs/rtp+tag+implementation) Settings（帐户设置）”下的RTP Tag（RTP标记）选项已更新为包括：

1. CDN和异步（推荐标记）
1. CDN和同步（高速）
1. 无CDN的异步标签
1. 无CDN的同步标签

为获得最佳性能，建议将标记放在网页后面标题的顶部 `<head>`。 所有标记都允许 [使用RTP API](http://developers.marketo.com/documentation/websites/rtp-js-api/)。 有关如何部署RTP标签的信息，请参 [阅此](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

![](assets/image2015-1-15-13-3a30-3a45.png)
