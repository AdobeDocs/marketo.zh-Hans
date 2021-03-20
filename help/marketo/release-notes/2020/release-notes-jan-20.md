---
unique-page-id: 37355534
description: 发行说明 — 2020年1月 — Marketo Docs — 产品文档
title: 发行说明 — 2020年1月
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---


# 发行说明：2020年1月{#release-notes-jan}

’20年1月版包含以下功能。 查看您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>由星形(![(star)](assets/star-yellow.svg))表示的特征是付费附加项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度发行_**

以下功能将于2020年1月17日&#x200B;**发布**。

## 核心Marketo EngageAdobe应用程序{#core-marketo-engage-adobe-application}

* [Adobe Experience Manager资产选择器](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/importing-assets-with-adobe-experience-manager.md):通过直接在Marketo Engage中提供的AEM资产快速访问与您的品牌相符的资产。注意：虽然我们的Marketo Sky体验和经典体验中都提供此功能，但经典体验中也提供管理功能。 您必须是AEM Assets的客户，并且版本必须为6.5或更高版本。

>[!NOTE]
>
>目前，仅Firefox完全支持AEM资产选择器。 Safari中不支持此功能，并且可能无法在最新版Chrome(v. 80)中工作，具体取决于您的SameSite Cookie设置。

* **Microsoft Dynamics — 实时同步导致CRM**:在Marketo Engage和Microsoft Dynamics之间实时同步潜在客户和联系人。创建潜在客户或联系人，并在Microsoft Dynamics中通过“将人与Microsoft同步”流动操作立即查看他们。
* **LinkedIn潜在客户代Forms附加字段映射**:从LinkedIn潜在客户代Forms捕获潜在客户数据，为销售和营销接触点创建更相关的体验。将隐藏字段、同意字段和测试潜在客户字段拉入Marketo Engage。
* **电子邮件模板依赖关系API**:获取资产列表，这些资产依赖电子邮件模板来了解潜在更改的范围以及模板的相关性可以更快地更改和删除。
* **多实例管理增强**:通过订阅的可滚动和字母顺序下拉菜单快速导航到所需的实例。

## 基于帐户的营销{#account-based-marketing}

![（星号）](assets/star-yellow.svg)

* **[新帐户发现(测试版](https://docs.marketo.com/x/WQA6Ag) ![)（星级）](assets/star-yellow.svg)**:使用“帐户分析”根据您的AI支持的理想目标模型发现您的ABM战略的新客户帐户。视图、选择和导入建议的新帐户及其基于人工智能的适应和意图数据指示器，它们在您的Marketo Engage潜在客户和用于反导目标的帐户数据库中尚不存在。 可立即向符合条件的帐户分析客户提供。

<br> 

**_在整个季度内发布_**

以下功能按非季度周期发布，将在未来几个月发布。

## 可见{#bizible}

![（星号）](assets/star-yellow.svg)

* **Marketo Engage潜在客户集成**:将销售和营销与统一的跨Bizible和Marketo Engage销售线索视图结合在一起。通过此更新，Marketo Engage现在可用作其他潜在客户数据源，因此您不必再等待潜在客户与CRM同步，即可报告潜在客户生成情况。
* **Discover增强功能**:通过从客户反馈开发的增强功能，从Bizible的Discover展示板中获得更多信息，例如从拼贴和属性中向下钻取到交易记录、添加基本记录计数和相应的每成本指标，以及为多个仪表板添加/删除仪表板过滤器。登录后，您还将直接转到默认仪表板。

## Marketo Sky{#marketo-sky}

* [图像编辑](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio):访问Adobe的编辑功能，而不必离开Marketo Engage。这一新功能可让您轻松执行诸如增强、裁切文本以及直接在Design Studio中向图像添加文本等操作。

## 销售分析{#sales-insight}

* **Salesforce闪电批量操作**:通过添加多达200个联系人/潜在活动并通过Salesforce Lightning批量向其发送Marketo Engage电子邮件，提高销售效率并吸引买家。
* **针对Salesforce的移动支持1**:您现在可以直接在Salesforce1应用程序中对所有Sales Insight功能(如“有趣的时刻”、Web活动和电子邮件)进行移动访问。
* **UI增强**:更新的界面，增强了可读性，设计符合我们的Marketo Sky体验。

## Sales Connect {#sales-connect}

* **网格组件**:使用新的网格自定义功能优化您的Sales Connect实例。选择要显示的列，搜索列，选择/取消选择所有列，并确定要在每个页面上查看多少行数据。
* **[内容锁定](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**:借助一个订阅范围的设置最大化品牌协调，该设置控制非管理员是否能够创建和编辑模板及活动。

>[!NOTE]
>
>* **TLS 1.0和1.1弃用**:为了与Adobe的发布结构进行持续的集成，我们将TLS 1.0和TLS 1.1的弃用改为2020年1月13日。有关详细信息，请在[此处](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)找到。
   >
   >
* **ITP 2.1+ Munchkin更新**:由于Safari的Cookie策略发生更改，ITP将限制Munchkin跨同一域上的会话跟踪用户的能力，这取决于访客使用的浏览器和浏览器版本，限制为1天或7天。为此，我们正在实施一项新的Web服务，以允许通过HTTP响应用Set-Cookie头设置Munchkin cookie。 有关如何实施此新服务的详细信息，请在[此处](https://nation.marketo.com/docs/DOC-7351)找到。


**_产品发_** [布网络](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 研讨会在3月3日上午11:00PT/下午2:00加入我们，参加由我们的产品团队主持的实时网络研讨会，了解有关此版本中包含的功能的更多信息。
