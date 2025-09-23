---
description: 发行说明 — 2021年8月 — Marketo文档 — 产品文档
title: 发行说明 - 2021 年 8 月
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 1%

---

# 发行说明：2021 年 8 月 {#release-notes-aug-21}

2021年8月版本中包含以下功能。 检查您的Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![](assets/yellow-star.png))表示的功能是付费加载项。 请联系您的Adobe Marketo Engage代表以了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2021年8月20日发布**。

## 体验自动化 {#experience-automation}

* **通过Marketo Engage Identity进行的Adobe用户身份验证**：不久将使用Adobe ID用户凭据载入新的具有Enterprise包的Marketo Engage用户。 到2022年年中，才将当前用户迁移到综合身份系统，在进一步通知之前，无需采取任何行动。 Adobe身份用户身份验证允许IT/安全管理员管理多个Marketo Engage产品实例及其他Experience Cloud解决方案，以及通过通用控制台配置SSO。 管理员可以方便地在一个位置管理用户组和用户权限。

* **可执行促销活动嵌套**：可执行促销活动现在还可以调用其他可执行促销活动，以便您嵌套至多三层深。 这能够进一步整合常见操作流程并改进Smart Campaign管理。

* **人员详细信息页面中的单流程操作**（9月9日前提供）：在不切换到数据库网格视图的情况下，使用流程操作菜单从人员详细信息页面对个人执行流程操作，如发送电子邮件、更改人员所有者或任何其他智能促销活动操作。

* **[自定义活动导出](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**：元数据导出现在支持可用于共享、分析和设计您的订阅数据模型的所有对象和相应的元数据。

## API增强功能 {#api-enhancements}

* **提交表单API**：当电子邮件地址在两个或更多Lead记录中重复时，我们会更新“上次更新”记录而不是完全跳过。 提供与Forms 2.0 API的对等功能。

* **电子邮件API**：检索冠军或挑战者电子邮件资产。 使用日期范围过滤器检索电子邮件资源。

**_在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

* **增强了Salesforce CRM用户的Lead、Contact、Account和Opportunity活动的可见性**：由于[!DNL Sales Insight]中的参与记录数量增加，在较长的销售周期内与潜在客户进行参与将更加有用。 有趣的时刻、Web活动、电子邮件和分数选项卡显示Lead、Contact、Account和Opportunity对象中多达400个活动。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **电子邮件连接限制(Beta)**：通过Sales Connect的电子邮件连接限制，提高电子邮件可投放性并扩展个性化销售通信。 这项新技术可自动管理电子邮件发送时间，为[!DNL Exchange]和Gmail用户创造无缝体验。 减少或取消使用第三方批量电子邮件发送应用程序，并放心地从[!DNL Sales Connect]发送您的所有电子邮件。

>[!NOTE]
>
>电子邮件限制功能现在可在Beta中使用。 [了解详情](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)。

* **增强的销售活动见解**：根据销售团队先前的活动捕获和激活个性化参与。 在Marketo Engage智能列表中可以使用新的属性，例如“销售呼叫记录链接”、“销售活动名称”和“销售电子邮件主题”。  这些活动可以通过Marketo Engage REST API或批量导出导出进行导出和报告，并作为智能列表的附加限制条件在筛选器和触发器上可用。

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible][!DNL LinkedIn]潜在客户Forms集成**：营销人员现在可以对在[!DNL LinkedIn]通过他们的潜在客户Forms广告单元捕获表单填写时发生的转化执行收入归因。 这些见解随后可用于优化表单性能和付费媒体投资。 [!DNL LinkedIn]潜在客户Gen Forms是[!DNL LinkedIn]增长最快的付费媒体产品之一，这项新功能包含在我们与[!DNL LinkedIn]的现有[!DNL Bizible]广告集成中。

* **改进了Velocity功能板**：我们新增了一个新的Velocity量度和功能板筛选器，以便获得更深入的见解。 营销人员使用此仪表板来了解分阶段潜在客户和商机周转率以及不同营销和销售参与形式的效率。

* **新同类群组瀑布历程仪表板**：这将使营销人员能够查看选定同类群组在经典“需求瀑布”阶段集中的进度，从而逐阶段快速了解转化率和隐含的阶段转化因果关系。

## [!DNL Bizible]与Adobe Experience Cloud集成 {#bizible-integration-with-adobe-experience-cloud}

此部分包含适用于已完成其Adobe Identity Management System (IMS)迁移的Bizible用户的新功能。 如果您已迁移，则将在Adobe ID选项卡下的[!DNL Bizible]设置中看到新的Adobe ID。 所有帐户都应在2021年底之前迁移。

* **[!DNL Bizible]与Adobe Privacy Service**&#x200B;的集成（2021年9月推出）： [!DNL Bizible]与Adobe Privacy Service的集成可跨Adobe Experience Cloud应用程序集中管理对关键数据隐私法规（如GDPR）的合规性。 现在，您可以利用此服务并集中管理所有隐私请求，以便跨应用程序反映传入[!DNL Bizible]和其他Adobe产品的更改请求。

* Adobe Unified Shell **[!DNL Bizible]上的**： [!DNL Bizible]采用Adobe Unified Shell为用户提供了新的功能，这些功能将显示在[!DNL Bizible]应用程序标题栏中，并包括更好地访问支持资源和应用程序切换。 Adobe Unified Shell有助于在[!DNL Bizible]和其他Adobe Experience Cloud应用程序之间创建一致的体验。

* **[!DNL Bizible]域所有权和自我管理**： [!DNL Bizible]用户可以利用Adobe Admin Console管理他们希望[!DNL Bizible]跟踪的域。 这可以为之前手动执行的流程引入自助服务，并提供有关如何跨Adobe Experience Cloud应用程序管理域所有权和跟踪的一致体验。

## 公告 {#announcements}

* **更新到订阅通用ID设置**：为了支持现有用户即将集成的Marketo Engage和Adobe标识，所有Marketo Engage订阅将在启用通用ID支持时统一起来。 可在此处[找到更多信息](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)。

**_产品发布网络研讨会_**

[2021年8月Marketo Engage发布网络研讨会](https://engage.marketo.com/August21_Release_Webinar.html)
