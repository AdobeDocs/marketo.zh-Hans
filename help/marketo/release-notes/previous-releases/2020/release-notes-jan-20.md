---
unique-page-id: 37355534
description: 发行说明 — 2020年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年1月
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 发行说明：2020年1月 {#release-notes-jan}

2020年1月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号( ![(star)](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将发布于 **2020年1月17日**.

## 核心Marketo EngageAdobe应用程序 {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager资源选择器](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md)：通过Marketo Engage中直接提供的AEM资源，快速访问与您的品牌相一致的资源。 注意：虽然此功能在Marketo Sky和经典体验中均可用，但可在我们的经典体验中找到管理功能。 您必须是AEM Assets的客户并且拥有版本6.5或更高版本。

>[!NOTE]
>
>目前，仅在Firefox中完全支持AEM资产选择器。 Safari不支持它，并且它可能不适用于最新版本的Chrome (v. 80)，具体取决于您的SameSite Cookie设置。

* **Microsoft Dynamics — 实时将潜在客户同步到CRM**：在Marketo Engage和Microsoft Dynamics之间实时同步潜在客户和联系人。 创建潜在客户或联系人，然后立即在Microsoft Dynamics中通过“将人员同步到Microsoft”流程操作查看它们。
* **linkedIn潜在客户Gen Forms其他字段映射**：从LinkedIn Lead Gen Forms中捕获潜在客户数据，为销售和营销接触点创建更相关的体验。 将隐藏字段、同意字段和测试潜在客户字段拉入Marketo Engage。
* **电子邮件模板依赖项API**：获取依赖于电子邮件模板的资源的列表以了解潜在更改的范围，并且可以更快地更改和删除对模板的依赖关系。
* **多实例管理增强功能**：使用订阅的可滚动按字母顺序下拉菜单，快速导航到所需的实例。

## Account-Based Marketing {#account-based-marketing}

![(star)](assets/yellow-star.png)

* **[新帐户发现（测试版）](https://docs.marketo.com/x/WQA6Ag) ![(star)](assets/yellow-star.png)**：使用帐户分析，根据由AI提供支持的理想客户配置文件模型发现ABM策略的新目标帐户。 查看、选择和导入推荐的新帐户，以及它们基于人工智能的适应和意图数据指示器，这些指示器在ABM定位的Marketo Engage商机和帐户数据库中尚不存在。 立即可供符合帐户分析客户资格条件的客户使用。

<br> 

**_将在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Marketo Engage潜在客户集成**：将销售和营销结合在一起，并统一查看跨Bizible和Marketo Engage的销售机会。 通过此更新，Marketo Engage现在可以用作额外的潜在客户数据源，因此您不再需要等待潜在客户与CRM同步来报告潜在客户生成。
* **发现增强功能**：利用根据客户反馈开发的增强功能，从我们的Discover Boards in Bizible中获取更多信息，例如从图块和属性深入到事务记录，添加基本记录计数和相应的每成本量度，以及为多个仪表板添加/删除仪表板筛选器的功能。 登录后，您还将直接转到默认信息板。

## Marketo Sky {#marketo-sky}

* [图像编辑](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio)：无需离开Marketo Engage即可访问Adobe的编辑功能。 这项新功能允许您直接在Design Studio中轻松执行增强、裁切和向图像添加文本等操作。

## 销售分析 {#sales-insight}

* **Salesforce闪电批量操作**：提高销售效率，让购买者能够添加最多200个营销活动联系人/潜在客户，并使用Salesforce Lightning批量向他们发送Marketo Engage电子邮件。
* **Salesforce1的移动支持**：您现在可以在Salesforce1应用程序中移动访问所有Sales Insight功能，如“有趣的时刻”和“Web活动和电子邮件”。
* **UI增强**：更新了界面，增强了可读性，并提供了与我们Marketo Sky体验一致的设计。

## Sales Connect {#sales-connect}

* **网格组件**：使用新的网格自定义功能优化您的Sales Connect实例。 选择要显示的列，搜索列，选择/取消选择所有列，并确定要在每个页面上查看多少行数据。
* **[内容锁定](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**：通过全订阅设置最大限度地实现品牌协调，该设置控制非管理员是否能够创建和编辑模板和营销活动。

>[!NOTE]
>
>* **弃用TLS 1.0和1.1**：为持续努力与Adobe的发布结构集成，我们将TLS 1.0和TLS 1.1的弃用时间转移到2020年1月13日。 可以找到更多详细信息 [此处](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **ITP 2.1+ Munchkin更新**：由于对Safari的Cookie策略进行了更改，Munchkin在同一域上跨会话跟踪用户的能力将被ITP限制为1天或7天，具体取决于访客使用的浏览器和浏览器版本。 为此，我们正在实施一项新的Web服务，以允许通过HTTP响应使用Set-Cookie标头设置Munchkin Cookie。 有关如何实施此新服务的更多信息，请参阅 [此处](https://nation.marketo.com/docs/DOC-7351).

**_产品发布网络研讨会_** [加入我们](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3月3日上午11:00（太平洋时间）/下午2:00（东部时间）举行的实时网络研讨会，由我们的产品团队主办，详细了解此版本中包含的功能。
