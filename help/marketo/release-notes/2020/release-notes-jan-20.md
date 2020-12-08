---
unique-page-id: 37355534
description: 发行说明- 2020年1月- Marketo Docs —— 产品文档
title: 发行说明- 2020年1月
translation-type: tm+mt
source-git-commit: 6f49037bf698b1646004720815897f992911f716
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---


# 发行说明：2020年1月 {#release-notes-jan}

2020年1月版包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!NOTE]
>
>**可用性**
>
>由星(（星）) ![表示的特征](assets/star-yellow.svg)，是付费附加项。 请联系您的Marketo Engage代表以了解更多信息。

***季度版本*** 2020年1月17日将发布 **以下功能**。

## 核心Marketo EngageAdobe应用 {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager资产选择器](https://docs.marketo.com/x/_AA6Ag):通过直接在Marketo Engage中提供的AEM资产快速访问与您的品牌相符的资产。 注意：虽然该功能在我们的Marketo Sky体验和经典体验中均可用，但在经典体验中可以找到管理功能。 您必须是AEM Assets的客户并且版本必须为6.5或更高版本。

>[!NOTE]
>
>目前，仅在Firefox中完全支持AEM资产选择器。 Safari中不支持此功能，并且它可能在最新版Chrome(v. 80)中无法使用，具体取决于您的SameSite cookie设置。

* **Microsoft Dynamics —— 同步实时引导CRM:** 在Marketo Engage和Microsoft Dynamics之间实时同步潜在客户和联系人。 创建潜在客户或联系人，并在Microsoft Dynamics中通过“将人员同步到Microsoft”流动操作立即查看他们。
* **LinkedIn潜在客户GenForms附加字段映射：** 从LinkedIn潜在客户代Forms获取潜在客户数据，为销售和营销接触点创建更相关的体验。 将隐藏字段、同意字段和测试潜在客户字段拉入Marketo Engage。
* **电子邮件模板依赖关系API**:获取资产列表，这些资产依赖电子邮件模板来了解潜在更改的范围，并且可以更快地更改和删除模板的地址相关性。
* **多实例管理增强功能**:使用订阅的可滚动和字母顺序下拉菜单快速导航到所需的实例。

基于帐户的营 ![销（星形）](assets/star-yellow.svg)

* [新帐户发现(测试版](https://docs.marketo.com/x/WQA6Ag) ) ![（星形）](assets/star-yellow.svg) :使用“帐户分析”根据您基于AI的理想客户目标模型发现ABM战略的新客户帐户。 视图、选择和导入建议的新帐户及其基于人工智能的拟合和意图数据指标，它们在您的Marketo Engage线索和用于反导瞄准的帐户数据库中尚不存在。 对符合资格的帐户分析客户可立即使用。

<br> 

## 新建部分

***整季度发布***

以下功能在非季度周期中发布，并将在未来几个月中发布。

Bizbile ![（星形）](assets/star-yellow.svg)

* **Marketo Engage潜在客户集成**:将销售和营销与统一的跨Bizible和Marketo Engage潜在客户视图结合在一起。 通过此更新，Marketo Engage现在可用作额外的潜在客户数据源，因此您不必再等待潜在客户与CRM同步，即可报告潜在客户生成。
* **发现增强**:通过从客户反馈开发的增强功能，从我们的Discover展示板中获得更多信息，如能够从拼贴和属性中向下钻取交易记录、添加基本记录计数和相应的每项成本指标，以及为多个仪表板添加／删除仪表板过滤器。 登录时，您还将直接转到默认仪表板。

## Marketo Sky  {#marketo-sky}

* [图像编辑](https://help.marketo.com/hc/en-us/articles/360041344614-Marketo-Image-Editor):访问Adobe的编辑功能，而无需离开Marketo Engage。 这一新功能可让您轻松地直接在Design Studio中对图像进行增强、裁切和添加文本等操作。

## 销售分析  {#sales-insight}

* **Salesforce闪电批量操作**:提高销售效率，并通过添加多达200个联系人／潜在顾客来吸引活动，并通过Salesforce Lightning向其批量发送Marketo Engage电子邮件来吸引买家。
* **Salesforce的移动支持1**:您现在可以直接在Salesforce1应用程序中访问所有Sales Insight功能，如“有趣的时刻”和“Web活动和电子邮件”。
* **UI增强**:更新的界面，增强了可读性，设计与我们的Marketo Sky体验保持一致。

## Sales Connect  {#sales-connect}

* **网格组件**:使用新的网格自定义功能优化您的Sales Connect实例。 选择要显示的列，搜索列，选择／取消选择所有列，并确定要在每页上查看多少行数据。
* [内容锁定](https://docs.marketo.com/x/6wA6Ag):通过控制非管理员是否能够创建和编辑模板及订阅的全活动设置，最大化品牌协调。

>[!NOTE]
>
>* **TLS 1.0和1.1弃用**:为了与Adobe的发布结构进行持续的集成，我们正在将TLS 1.0和TLS 1.1的弃用改为2020年1月13日。 更多详细信息可在此 [找到](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)。
   >
   >
* **ITP 2.1+ Munchkin更新**:由于Safari的cookie策略发生了更改，Munchkin在同一域上跨会话跟踪用户的能力将受ITP限制，期限为1天或7天，这取决于访客使用的浏览器和浏览器版本。 为此，我们实施了新的Web服务，允许通过HTTP响应使用Set-Cookie头设置Munchkin cookie。 有关如何实施此新服务的更多信息，请参 [阅](https://nation.marketo.com/docs/DOC-7351)。


***产品发布网络*** 研讨会3月 [](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3日上午11:00PT /下午2:00PM加入我们，参加由我们的产品团队主持的实时网络研讨会，了解有关此发行版包含的功能的更多信息。
