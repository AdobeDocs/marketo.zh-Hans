---
unique-page-id: 37355534
description: 发行说明 — 2020年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年1月
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# 发行说明：2020年1月 {#release-notes-jan}

2020年1月版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![（星号）](assets/yellow-star.png))表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2020年1月17日**&#x200B;发布。

## 核心Marketo Engage Adobe应用程序 {#core-marketo-engage-adobe-application}

* [Adobe Experience Manager资源选择器](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md)：快速访问与您的品牌相符的资源，这些资源可直接在Marketo Engage中使用AEM资源。 注意：虽然此功能在我们的Marketo Sky和经典体验中均可用，但可在我们的经典体验中找到管理功能。 您必须是AEM Assets的客户并且拥有版本6.5或更高版本。

>[!NOTE]
>
>目前，仅在Firefox中完全支持AEM资产选择器。 Safari不支持它，并且它可能不适用于最新版本的Chrome (v. 80)，具体取决于您的SameSite Cookie设置。

* **[!DNL Microsoft Dynamics]— 将潜在客户实时同步到CRM**：在Marketo Engage和[!DNL Microsoft Dynamics]之间实时同步潜在客户和联系人。 创建潜在客户或联系人，然后立即在[!DNL Microsoft Dynamics]中通过“将人员同步到Microsoft”流程操作查看它们。
* **[!DNL LinkedIn]潜在客户Gen Forms附加字段映射**：从[!DNL LinkedIn]潜在客户Gen Forms中捕获潜在客户数据，以便为销售和营销接触点创建更相关的体验。 将隐藏字段、同意字段和测试潜在客户字段拉入Marketo Engage。
* **电子邮件模板依赖项API**：获取依赖于电子邮件模板的资源的列表，以了解可能的更改范围，并且可以更快地更改和删除对模板的依赖项。
* **多实例管理增强功能**：使用订阅的可滚动按字母顺序排序的下拉菜单，快速导航到所需的实例。

## Account-Based Marketing {#account-based-marketing}

![（星形）](assets/yellow-star.png)

* [新帐户发现(BETA)](https://docs.marketo.com/x/WQA6Ag) ![(star)](assets/yellow-star.png)：使用帐户分析，根据由AI提供支持的理想客户配置文件模型，为ABM策略发现全新目标帐户。 查看、选择和导入推荐的新帐户，以及这些基于人工智能的拟合和意图数据指示器，您的Marketo Engage潜在客户和帐户数据库中尚未存在这些用于ABM定位的新帐户。 立即可供符合帐户分析客户资格条件的客户使用。

<br> 

**_在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## [!DNL Bizible] {#bizible}

![（星形）](assets/yellow-star.png)

* **Marketo Engage潜在客户集成**：将销售和营销以及跨[!DNL Bizible]和Marketo Engage的潜在客户统一视图整合在一起。 通过此更新，Marketo Engage现在可以用作额外的潜在客户数据源，因此您不再需要等待潜在客户与CRM同步来报告潜在客户生成。
* **发现增强功能**：通过根据客户反馈开发的增强功能，从[!DNL Bizible]中的发现展示板中获取更多信息，例如，从图块和属性向下钻取到事务记录，添加基本记录计数和相应的每成本量度，以及为多个仪表板添加/删除仪表板筛选器的功能。 登录后，您还将直接转到默认信息板。

## [!DNL Marketo Sky] {#marketo-sky}

* [图像编辑](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=zh-Hans#design-studio)：无需离开Adobe即可访问Marketo Engage的编辑功能。 这项新功能允许您轻松地直接在[!UICONTROL Design Studio]中增强、裁切文本并将其添加到图像。

## [!DNL Sales Insight] {#sales-insight}

* **[!DNL Salesforce Lightning]批量操作**：提高销售效率并使购买者能够持续参与，从而向营销活动添加最多200个联系人/潜在客户，并批量向他们发送带有[!DNL Salesforce Lightning]的Marketo Engage电子邮件。
* **针对[!DNL Salesforce1]**&#x200B;的移动支持：您现在可以在[!DNL Salesforce1]应用程序中移动访问所有[!DNL Sales Insight]功能，如“有趣的时刻”和“Web活动和电子邮件”。
* **UI增强**：更新了界面，增强了可读性，并提供了与我们[!DNL Marketo Sky]体验一致的设计。

## [!DNL Sales Connect] {#sales-connect}

* **网格组件**：使用新的网格自定义功能优化您的[!DNL Sales Connect]实例。 选择要显示的列，搜索列，选择/取消选择所有列，并确定要在每个页面上查看多少行数据。
* **[内容锁定](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**：通过全订阅设置（控制非管理员是否能够创建和编辑模板和营销活动）最大限度地实现品牌一致性。

>[!NOTE]
>
>* **TLS 1.0和1.1弃用**：为继续与Adobe的版本结构集成，我们已将弃用的TLS 1.0和TLS 1.1转移到2020年1月13日。 更多详细信息可在[此处](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq)找到。
>
>* **ITP 2.1+ [!DNL Munchkin]更新**：由于对[!DNL Safari]的Cookie策略进行了更改，[!DNL Munchkin]在同一域上跨会话跟踪用户的能力将被ITP限制为1天或7天，具体取决于访客使用的浏览器和浏览器版本。 为此，我们正在实施一项新的Web服务，以允许通过HTTP响应使用Set-Cookie标头设置Munchkin Cookie。 有关如何实施此新服务的详细信息，可在[此处](https://nation.marketo.com/docs/DOC-7351)找到。

**_产品发布网络研讨会_** [与我们](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html)一起参加我们于3月3日太平洋时间上午11:00/下午2:00举行的实时网络研讨会，该研讨会由我们的产品团队主持，详细了解此版本中包含的功能。
