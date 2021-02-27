---
unique-page-id: 4720758
description: 发行说明 — 2015年1月 — Marketo Docs — 产品文档
title: 发行说明 — 2015年1月
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---


# 发行说明：2015年1月{#release-notes-january}

2015年1月版包含以下功能。 请查看您的Marketo Edition以了解功能可用性。 发布后，请务必回来查找每个功能的详细文章的链接！

## 营销自动化更新{#marketing-automation-updates}

**移动友好登陆页**

您现在可以从登陆页编辑器中[为登陆页](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md)构建移动视图。 无论使用何种设备，都能有效地传递您的信息，并通过定制内容以随时随地轻松消费来提高参与度。 此功能将在发行后的一周内逐步推出。

[-登陆页视频演练 — ](https://youtu.be/aPQHlG2X6c0)

**新Rest API调用**

对Lead &amp; 活动 ReST API的三个新调用：

* 删除潜在客户
* 通过项目ID获取潜在客户
* 获取已删除的潜在客户

此外，同步潜在客户还有一个新选项，可异步写入潜在客户更改以进行更快的API调用。 发行版[developers.marketo.com](https://developers.marketo.com)后将提供完整的详细信息

**电子邮件脚本自定义对象支持**

现在从电子邮件脚本中访问与Account对象关联的自定义对象！

## 实时个性化{#real-time-personalization}

**针对Google和Facebook的个性化再营销**

再营销向访问过您网站的人员显示广告。 您现在可以使用来自实时个性化的数据在[Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)和[Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)上个性化您的再营销活动。 向来自不同行业的受众、指定帐户列表、公司规模或任何已知潜在客户数据进行再营销。

[指定帐户列表模块](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

对“指定帐户”模块的增强将提高用户的匹配率和验证。 新增包括：

* 使用潜在客户的电子邮件地址(也适用于仅RTP列表的客户)匹配指定帐户中的组织
* 支持每个帐户最多10万条记录
* 要视图和下载的CSV文件模板

![](assets/image2015-1-14-11-3a12-3a16.png)

**更新的RTP标签选项**

“帐户设置”下的RTP标记选项已更新为包括：

1. CDN和异步（推荐标签）
1. CDN和同步（高速）
1. 无CDN的异步标签
1. 无CDN的同步标签

为获得最佳性能，建议将标记放在`<head>`之后网页标题的顶部。 所有标记都允许使用[RTP API](https://developers.marketo.com/documentation/websites/rtp-js-api/)。 有关如何部署RTP标签的信息，请参阅[此处](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

![](assets/image2015-1-15-13-3a30-3a45.png)
