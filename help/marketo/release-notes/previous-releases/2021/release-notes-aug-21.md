---
description: 发行说明 — 2021年8月 — Marketo文档 — 产品文档
title: 发行说明 — 2021年8月
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 发行说明：2021年8月 {#release-notes-aug-21}

2021年8月版中包括以下功能。 检查您的Marketo Engage版本，了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![](assets/yellow-star.png))是付费加载项。 请联系您的Adobe Marketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将发布于 **2021年8月20日**.

## 体验自动化 {#experience-automation}

* **通过Adobe身份进行Marketo Engage用户身份验证**：不久，将使用Adobe ID用户凭据载入具有企业包的新Marketo Engage用户。 到2022年年中才能将当前用户迁移到综合身份系统，在进一步通知之前无需采取任何行动。 Adobe身份用户身份验证允许IT/安全管理员管理多个Marketo Engage产品实例及其他Experience Cloud解决方案，以及通过通用控制台配置SSO。 管理员可以方便地在一个位置管理用户组和用户权限。

* **可执行的Campaign嵌套**：可执行营销活动现在还可以调用其他可执行营销活动，以便您将其嵌套至最多三层深。 这有助于进一步整合常见操作流程并改进Smart Campaign管理。

* **“人员详细信息”页中的单流程活动** （9月9日前提供）：在不切换到数据库网格视图的情况下，使用流程操作菜单执行流程操作，如发送电子邮件、更改人员所有者或对人员详细信息页面中的个人执行任何其他智能促销活动操作。

* **[自定义活动导出](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**：元数据导出现在支持可用于共享、分析和设计订阅数据模型的所有对象和相应的元数据。

## API增强功能 {#api-enhancements}

* **提交表单API**：当电子邮件地址在两个或更多Lead记录中重复时，我们更新“上次更新”记录而不是完全跳过。 提供与Forms 2.0 API的等同功能。

* **电子邮件API**：检索冠军或挑战者电子邮件资产。 使用日期范围过滤器检索电子邮件资源。

**_整个季度发布_**

以下功能属于非季度周期，将在未来几个月发布。

## 销售分析 {#sales-insight}

![(star)](assets/yellow-star.png)

* **增强了Salesforce CRM用户的Lead 、 Contact 、 Account和Opportunity活动的可见性**：由于Sales Insight中的参与记录数量增加，因此在较长的销售周期内与潜在客户接洽会更了解情况。 有趣的时刻、Web活动、电子邮件和分数选项卡显示Lead、Contact、Account和Opportunity对象中多达400个活动。

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **电子邮件连接限制（测试版）**：通过Sales Connect的电子邮件连接限制，提高电子邮件可投放性并扩展个性化的销售通信。 这项新技术可自动管理电子邮件发送时间，为Exchange和Gmail用户创造无缝体验。 减少或不再使用第三方批量电子邮件发送应用程序，放心地从Sales Connect发送所有电子邮件。

>[!NOTE]
>
>电子邮件限制功能现在在Beta版中可用。 [了解详情](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **增强的销售活动分析**：根据您的销售团队以前的活动，捕获和激活个性化的参与。 可以在Marketo Engage智能列表中使用新的属性，例如Sales Call Recording Link 、 Sales Campaign Name和Sales Email Subject。  这些活动可以通过Marketo EngageREST API或批量导出导出进行导出和报告，并可在筛选器和触发器上用作智能列表的附加约束。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms集成**：营销人员现在可以对LinkedIn捕获表单填充时发生的转化执行收入归因，这体现在他们的Forms潜在客户广告单元中。 然后，这些见解可用于优化表单性能和付费媒体投资。 linkedIn Lead Gen Forms是LinkedIn增长最快的付费媒体产品之一，这项新功能包含在我们与Bizible的现有LinkedIn Ads集成中。

* **改进了Velocity功能板**：我们新增了速度量度和功能板过滤器，以便获得更深入的见解。 营销人员使用此仪表板来了解分阶段销售线索和机会周转率，以及不同形式的营销和销售活动的效率。

* **新的同类群组瀑布历程功能板**：营销人员将可以通过一组经典的“需求瀑布”阶段查看选定同类群组的进度，从而逐阶段快速了解转化率和隐含的阶段转化因果关系。

## Bizible与Adobe Experience Cloud集成 {#bizible-integration-with-adobe-experience-cloud}

此部分包含适用于已完成其AdobeIdentity Management System (IMS)迁移的Bizible用户的新功能。 如果您已迁移，则将在Adobe ID选项卡下的Bizible设置中看到新的Adobe ID。 所有帐户都应在2021年底之前迁移。

* **Bizible与AdobePrivacy Service集成** （2021年9月推出）：Bizible与AdobePrivacy Service的集成实现了跨Adobe Experience Cloud应用程序对关键数据隐私法规（如GDPR）的集中遵守。 现在，您可以利用此服务并集中管理所有隐私请求，以便提交到Bizible和其他Adobe产品的更改请求能够跨应用程序反映出来。

* **Adobe Experience Cloud界面上的Bizible**： Bizible采用Adobe Experience Cloud界面，为用户提供了新功能，这些新功能将显示在Bizible应用程序标题栏中，并包括更好地访问支持资源和应用程序切换。 Experience Cloud界面有助于在Bizible和其他Adobe Experience Cloud应用程序之间创建一致的体验。

* **Bizible域所有权和自我管理**：Bizible用户可以利用Adobe Admin Console管理他们希望Bizible跟踪的域。 这可以为之前手动执行的流程引入自助服务，并提供有关如何跨Adobe Experience Cloud应用程序管理域所有权和跟踪的一致体验。

## 公告 {#announcements}

* **更新了订阅通用ID设置**：为了支持现有用户即将推出的Marketo Engage和Adobe身份集成，所有Marketo Engage订阅将在启用通用ID支持时统一起来。 更多信息 [可在此处找到](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_产品发布网络研讨会_**

[2021年8月Marketo Engage发布网络研讨会](https://engage.marketo.com/August21_Release_Webinar.html)
