---
unique-page-id: 6094890
description: 发行说明- 2015年2月- Marketo Docs —— 产品文档
title: 发行说明- 2015年2月
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---


# 发行说明：2015年2月 {#release-notes-february}

2015年2月版包含以下功能。 请查看您的Marketo Edition以了解功能可用性。 发布后，请务必返回以找到每个功能的详细文章的链接。 滚鼓……

## 营销自动化增强 {#marketing-automation-enhancements}

**移 [动智能活动](../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

欢庆！ 现在，您可以使用拖放或树中的移动功能在项目中移入和移出智能活动。

** [Dynamics 2015（在线）](http://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises) **-支持！

**HTTPS证书更改**

为保护客户数据和SaaS服务的机密性和完整性，营销人员应遵循SaaS行业最佳实践

并将以下域的当前使用的安全协议（SHA-1和SSL）替换为更安全的版本(SHA-2（即SHA-256）和TLS):

`·` [marketo.net](http://marketo.net) （加密的Munchkin流量）

`·` [marketo.com](http://marketo.com) （主SaaS应用程序）

此版本发布后不久将发生。 在2015年12月之前，SHA-1协 [议将在mktoapi.com域上临时受支持](http://mktoapi.com) ，以允许传统系统和应用程序的所有者使用SHA-2兼容性更新其系统。

**安全蒙奇金**

我们将删除对SSL3的支持。 我们一直在维护SSL3以保持对旧版Web浏览器的支持，但在2015年，我们不再看到来自这些浏览器的大量Web流量。 这在安全页面上使用时只会影响Munchkin，在2月发布后将缓慢推出。

## 实时个性化增强 {#real-time-personalization-enhancements}

** [目标URL](../../product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用“添加活动URL”选择您希望实时目标显示的页面。 此功能适用于所有活动类型（对话框、区域内构件、构件），但对于活动将仅在所选目标URL的区域ID中呈现的区域活动，此功能尤其有价值。 它支持向目标不同网页添加多个URL。

![](assets/image2015-2-19-11-3a0-3a30.png)

**国 [家／地区和州已加入基于帐户的定位](https://docs.marketo.com/display/DOCS/View+a+Named+Account+List)**

现在可以将国家／地区和州添加到您的指定帐户列表。 目标特定位置的密钥帐户潜在客户。
