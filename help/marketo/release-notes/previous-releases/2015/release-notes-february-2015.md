---
unique-page-id: 6094890
description: 发行说明 — 2015年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 发行说明：2015年2月 {#release-notes-february}

2015年2月版本中包含以下功能。 请检查您的Marketo版本是否提供了相关功能。 发布后，请务必返回以查找每个功能的详细文章链接。 鼓卷……

## 营销自动化增强功能 {#marketing-automation-enhancements}

**[移动智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

欢乐啊！ 现在，您可以使用拖放或树中的“移动”功能在项目中或项目中移动智能营销活动。

**[Dynamics 2015（在线）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — 支持！

**HTTPS证书更改**

为了保护客户数据和SaaS服务的机密性和完整性，Marketo遵循SaaS行业最佳实践

对于以下域，和将用更安全的版本(SHA-2（也称为SHA-256）和TLS)替换当前使用的安全协议（SHA-1和SSL）：

* marketo.net （加密的Munchkin流量）

* [marketo.com](https://marketo.com) （主要SaaS应用程序）

此版本发布后不久就会发生这种情况。 SHA-1协议将暂时受支持 [mktoapi.com](https://mktoapi.com) 到2015年12月为止的域名，允许旧版系统和应用程序的所有者更新其系统以使其兼容SHA-2。

**安全Munchkin**

我们将停止对SSL3的支持。 我们一直使用SSL3来保持对旧版Web浏览器的支持，但在2015年，我们不再看到来自这些浏览器的大量Web流量。 这仅会影响Munchkin（在安全页面上使用），并且在2月版发布后会缓慢推出。

## 实时个性化增强功能 {#real-time-personalization-enhancements}

**[营销活动的目标URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用“添加目标URL”选择您希望实时营销活动显示的页面。 此功能适用于所有营销活动类型（对话框、区域内部构件、小组件），但对于区域内部营销活动尤其有用，因为在该营销活动中，营销活动将仅在区域ID中针对选定的目标URL呈现。 它支持添加多个URL以定位不同的网页。

![](assets/image2015-2-19-11-3a0-3a30.png)

**添加到基于帐户的定位中的国家和州/省**

现在可以将国家/地区和省/市/自治区添加到您的指定帐户列表。 从特定位置定位关键客户潜在客户。
