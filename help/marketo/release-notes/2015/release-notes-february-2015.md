---
unique-page-id: 6094890
description: 发行说明 — 2015年2月 — Marketo Docs — 产品文档
title: 发行说明 — 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 发行说明：2015年2月{#release-notes-february}

2015年2月版包含以下功能。 请查看Marketo版以了解功能可用性。 发布后，请务必回来查找每个功能的详细文章的链接。 滚鼓……

## 营销自动化增强{#marketing-automation-enhancements}

**[移动智能活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

欢庆！ 现在，您可以使用拖放或树中的“移动”功能在项目中移入和移出智能活动。

**[支持Dynamics 2015(在线](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** )!

**HTTPS证书更改**

为保护客户数据和SaaS服务的机密性和完整性，Marketo遵循SaaS行业最佳实践

并将以下域的当前使用的安全协议（SHA-1和SSL）替换为更安全的版本(SHA-2（即SHA-256和TLS）：

* [marketo.net](https://marketo.net) （加密的Munchkin流量）

* [marketo.com](https://marketo.com) （主SaaS应用程序）

此版本发布后不久即会发生。 在2015年12月之前，[mktoapi.com](https://mktoapi.com)域上将暂时支持SHA-1协议，以允许旧系统和应用程序的所有者以SHA-2兼容性更新其系统。

**安全蒙奇金**

我们将取消对SSL3的支持。 我们一直维护SSL3，直到现在，以保持对旧Web浏览器的支持，但在2015年，我们不再看到来自这些浏览器的显着Web流量。 仅当在安全页面上使用时，这会影响Munchkin，并且在2月发布后将缓慢推出。

## 实时个性化增强{#real-time-personalization-enhancements}

**[目标的URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用“添加活动URL”选择希望实时目标显示的页面。 此功能适用于所有活动类型（对话框、区域、构件），但对于活动将仅在所选目标URL的区域ID中呈现的区域活动，此功能特别有用。 它支持向目标不同网页添加多个URL。

![](assets/image2015-2-19-11-3a0-3a30.png)

**添加到基于帐户的定位的国家/地区和州**

现在，可以将国家和州添加到您的指定帐户列表。 目标特定位置的密钥帐户潜在客户。
