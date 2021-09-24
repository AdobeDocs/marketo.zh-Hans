---
unique-page-id: 6094890
description: 发行说明 — 2015年2月 — Marketo文档 — 产品文档
title: 发行说明 — 2015年2月
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 发行说明：2015年2月 {#release-notes-february}

2015年2月版中包含以下功能。 请查看您的Marketo版以了解功能的可用情况。 发布后，请务必返回以查找指向每个功能详细文章的链接。 鼓卷……

## 营销自动化增强功能 {#marketing-automation-enhancements}

**[移动智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

欢庆！ 现在，您可以使用拖放或树中的移动功能，将智能营销活动移入和移出项目。

**[Dynamics 2015（在线）](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  — 支持！

**HTTPS证书更改**

为保护客户数据和SaaS服务的机密性和完整性，Marketo遵循SaaS行业最佳实践

和将用以下域的更安全版本(SHA-2（即SHA-256）和TLS)替换当前使用的安全协议（SHA-1和SSL）：

* [marketo.net](https://marketo.net) （加密的Munchkin流量）

* [marketo.com](https://marketo.com) （主SaaS应用程序）

此操作将在此版本发布后不久发生。 在2015年12月之前，将在[mktoapi.com](https://mktoapi.com)域上临时支持SHA-1协议，以允许旧版系统和应用程序的所有者使用SHA-2兼容性更新其系统。

**安全蒙奇金**

我们将删除对SSL3的支持。 我们一直维护SSL3以保持对旧Web浏览器的支持，但在2015年，我们不再看到这些浏览器带来的大量Web流量。 这仅会在安全页面上使用时影响Munchkin，并且在2月版发布后会缓慢推出。

## 实时个性化增强功能 {#real-time-personalization-enhancements}

**[营销活动的Target URL](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

使用“添加目标URL”选择您希望实时营销活动在中显示的页面。 此功能适用于所有营销活动类型（对话框、区域内、小组件），但对于区域内营销活动特别有价值，因为区域内营销活动将仅在选定目标URL的区域ID中呈现。 它支持添加多个URL以定位不同的网页。

![](assets/image2015-2-19-11-3a0-3a30.png)

**在基于帐户的定位中添加了国家/地区和州**

现在，可以将国家/地区和州添加到您的指定帐户列表中。 从特定位置定位关键帐户潜在客户。
