---
unique-page-id: 37355534
description: 发行说明 — 2020年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年1月
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
source-git-commit: 153c6a05be7ef94a0bc8b591b8f2eebdf879c5db
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 发行说明：2020年1月 {#release-notes-jan}

’20年1月版中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

>[!AVAILABILITY]
>
>由星( ![（星号）](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

将在 **2020年1月17日**.

## 核心Marketo EngageAdobe应用程序 {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager资产选择器](/help/marketo/product-docs/adobe-experience-cloud-integrations-overview/importing-assets-with-adobe-experience-manager.md):快速访问与您的品牌相符的资产，以便直接在Marketo Engage中提供AEM资产。 注意：虽然此功能在我们的Marketo Sky体验和经典体验中均可用，但在我们的经典体验中可以找到管理功能。 您必须是AEM Assets的客户，并且具有版本6.5或更高版本。

>[!NOTE]
>
>目前，只有Firefox完全支持AEM资产选择器。 Safari不支持此功能，并且根据您的SameSite Cookie设置，它可能在最新版本的Chrome（版本80）中不起作用。

* **Microsoft Dynamics — 实时同步潜在客户到CRM**:在Marketo Engage和Microsoft Dynamics之间实时同步潜在客户和联系人。 通过“将人员同步到Microsoft”流程操作，可立即在Microsoft Dynamics中创建潜在客户或联系人并查看他们。
* **linkedIn Lead Gen Forms其他字段映射**:从LinkedIn Lead Gen Forms中捕获潜在客户数据，以便为销售和营销接触点创建更相关的体验。 将隐藏字段、同意字段和测试潜在客户字段提取到Marketo Engage。
* **电子邮件模板依赖项API**:获取依赖于电子邮件模板的资产列表，以了解潜在更改的范围以及可以更快地更改和删除模板的地址依赖关系。
* **多实例管理增强功能**:使用订阅的可滚动和按字母顺序排列的下拉菜单快速导航到所需的实例。

## Account-Based Marketing {#account-based-marketing}

![（星号）](assets/yellow-star.png)

* **[新帐户发现（测试版）](https://docs.marketo.com/x/WQA6Ag) ![（星号）](assets/yellow-star.png)**:使用“帐户分析”根据您的AI支持的理想客户档案模型，为您的ABM战略发现新的目标帐户。 查看、选择和导入建议的新帐户，以及其基于人工智能的拟合和意图数据指标，这些指标在您的Marketo Engage线索数据库和用于反导定位的帐户数据库中不存在。 立即可供符合条件的帐户分析客户使用。

<br> 

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

## Bizible {#bizible}

![（星号）](assets/yellow-star.png)

* **Marketo Engage潜在客户集成**:将销售和营销与Bizible和Marketo Engage中销售线索的统一视图相结合。 通过此更新，Marketo Engage现在可用作额外的潜在客户数据源，因此您不必再等待潜在客户与CRM同步，即可报告潜在客户生成情况。
* **Discover增强功能**:通过从客户反馈开发的增强功能，从Bizible的Discover展示板获取更多信息，例如能够从图块和属性向下钻取到事务记录，添加基本记录计数和相应的每个成本量度，以及为多个功能板添加/删除功能板过滤器。 登录后，您还将直接转到默认功能板。

## Marketo Sky {#marketo-sky}

* [图像编辑](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio):无需离开Adobe即可访问其编辑功能。 通过这项新功能，您可以轻松地在Design Studio中直接对图像执行增强、裁剪和添加文本等操作。

## 销售分析 {#sales-insight}

* **Salesforce闪电批量操作**:提高销售效率，使购买者能够与多达200个联系人/潜在客户一起参与促销活动，并使用Salesforce Lightning批量向他们发送Marketo Engage电子邮件。
* **移动设备支持Salesforce1**:现在，您可以在Salesforce1应用程序中随时通过移动设备访问所有Sales Insight功能，如“有趣的时刻”和“Web活动和电子邮件”。
* **UI增强功能**:更新了界面，增强了可读性，并且设计与我们的Marketo Sky体验一致。

## Sales Connect {#sales-connect}

* **网格组件**:使用新的网格自定义功能优化您的Sales Connect实例。 选择要显示的列、搜索列、选择/取消选择所有列，并确定要在每个页面上查看多少行数据。
* **[内容锁定](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**:通过全订阅设置最大限度地协调品牌，该设置可控制非管理员是否能够创建和编辑模板和营销策划。

>[!NOTE]
>
>* **弃用TLS 1.0和1.1**:为了与Adobe的发行结构集成，我们将继续将TLS 1.0和TLS 1.1的弃用版本转移到2020年1月13日。 可以找到更多详细信息 [此处](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **ITP 2.1+ Munchkin更新**:由于Safari的Cookie策略发生了更改，ITP将根据访客使用的浏览器和浏览器版本，将限制Munchkin在同一域上跨会话跟踪用户的功能（1天或7天）。 为此，我们实施了新的Web服务，以允许通过HTTP响应使用Set-Cookie标头来设置Munchkin Cookie。 有关如何实施此新服务的详细信息，请参阅 [此处](https://nation.marketo.com/docs/DOC-7351).


**_产品发行网络研讨会_** [加入我们](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3月3日上午11:00 PT / 2:00 PM ET，由我们的产品团队主办的实时网络研讨会，了解有关此版本中包含的功能的更多信息。
