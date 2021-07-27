---
description: 最新发行说明 — Marketo文档 — 产品文档
title: 最新发行说明
source-git-commit: 97f6aeeb5c808df780b9b7bafd1bea5b1b805e5a
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 0%

---

# 发行说明：2021年8月 {#release-notes-aug-21}

’21年8月版中包含以下功能。 查看Marketo Engage版本以了解功能的可用性。

>[!AVAILABILITY]
>
>以星形(![](assets/yellow-star.png))表示的功能是付费的附加组件。 请联系您的AdobeMarketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将于2021年8月20日&#x200B;**发布。**

## Adobe Experience Platform集成 {#adobe-experience-platform-integration}

* **Marketo Engage通过Adobe身份进行用户身份验证**:从2021年9月起，将使用Adobe ID用户凭据载入具有企业包的新Marketo Engage用户。2022年年中之前，不会将当前用户迁移到集成身份系统，在收到进一步通知之前，也无需采取任何操作。 Adobe身份用户身份验证允许IT/安全管理员管理多个Marketo Engage产品实例以及其他Experience Cloud解决方案，并通过通用控制台配置单点登录。 管理员可以在一个位置方便地管理用户组和用户权限。

## 体验自动化 {#experience-automation}

* **可执行促销活动嵌套**:可执行促销活动现在还可以调用其他可执行促销活动，以便您将它们嵌套到最多三层深度。这可以进一步整合常用的操作流程，并改进智能营销活动管理。

* **“人员详细信息”页面中的单一流量操作**:使用“流程操作”菜单，从“人员详细信息”页面对个人执行流程操作（如发送电子邮件、更改人员所有者或任何其他智能营销活动操作），而无需切换到数据库网格视图。

* **自定义活动导出**:元数据导出现在支持所有对象和相应的元数据，这些对象和元数据可用于共享、分析和设计订阅数据模型。

## API增强功能 {#api-enhancements}

* **自定义字段元数据API**:简化合作伙伴集成Marketo Engage中自定义字段的创建和管理。自动在潜在客户对象上创建新字段，并立即和同时在多个Marketo Engage实例中更新字段。

* **增强的过滤**:现在，有几个API支持更多过滤，例如向电子邮件资产和项目群成员字段添加日期范围过滤器。现在，您只能提取在以下API的特定时间范围内更新的数据……
   * 获取项目成员
   * 获取电子邮件
   * 批量活动提取

* **提交表单API**:当一个电子邮件地址复制到两个或更多潜在客户记录中时，我们会更新“上次更新”记录，而不是完全跳过。与Forms 2.0 API相同。

* **电子邮件API**:检索冠军或挑战者电子邮件资产。

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

## 销售分析 {#sales-insight}

![（星号）](assets/yellow-star.png)

* **增强了Salesforce CRM用户对潜在客户、联系、帐户和机会活动的可见性**:由于Sales Insight中的参与记录数量增加，因此在较长的销售周期中与潜在客户的参与情况会得到更多了解。有趣的时刻、Web活动、电子邮件和分数选项卡在潜在客户、联系人、帐户和机会对象中显示了多达400个活动。

## Sales Connect {#sales-connect}

![（星号）](assets/yellow-star.png)

* **电子邮件连接限制(GA)**:通过对Sales Connect的电子邮件连接限制，提高电子邮件投放能力并扩展个性化销售通信。这项新技术可自动管理电子邮件发送时间，为Exchange和Gmail用户创建无缝体验。 减少或消除使用第三方批量电子邮件发送应用程序的情况，并满怀信心地从Sales Connect发送所有电子邮件。

* **增强的销售活动分析**:根据您销售团队的先前活动捕获并激活个性化参与。新属性（如“销售拜访记录链接”、“销售活动名称”和“销售电子邮件主体”）可在Marketo Engage智能列表中使用。  这些活动可以通过Marketo EngageREST API或批量导出进行导出和报告，并可在过滤器和触发器上作为智能列表的其他限制使用。

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms集成**:现在，营销人员可以对当LinkedIn通过其商机拓展Forms广告单元捕获表单填充时发生的转化执行收入归因。然后，可以使用这些分析来优化表单性能和付费媒体投资。 linkedIn领先代Forms是LinkedIn增长最快的付费媒体产品之一，此新功能包含在我们与Bizible的现有LinkedIn Ads集成中。 
 
* **改进了Velocity功能板**:我们新增了速度量度和功能板过滤器，以便提供更深入的分析。营销人员使用此功能板来了解逐阶段商机和销售机会的速度，以及不同营销和销售参与形式的效率。

* **新的同类群组瀑布图历程功能板**:这将使营销人员能够通过经典的“需求瀑布”阶段集来查看选定同类群组的进展，从而逐个快速了解转化率和隐含的阶段转化因果关系。

## Bizible与Adobe Experience Cloud集成 {#bizible-integration-with-adobe-experience-cloud}

此部分包含已完成其AdobeIdentity Management系统(IMS)迁移的Bizible用户的新功能。 如果您已迁移，您将在Adobe ID选项卡下的Bizible设置中看到新的Adobe ID。 所有帐户应在2021年底之前迁移。

* **Bizible与AdobePrivacy Service集成** （2021年9月提供）：Bizible与AdobePrivacy Service的集成可跨Adobe Experience Cloud应用程序集中遵守关键数据隐私法规（如GDPR）。您现在可以利用此服务并集中管理所有隐私请求，以便跨应用程序反映进入Bizible和其他Adobe产品的更改请求。

* **Adobe统一Shell上的Bizible**:Bizible采用Adobe统一Shell为用户提供了将显示在Bizible应用程序标题栏中的新功能，并包括更好地访问支持资源和应用程序切换。Adobe统一Shell有助于在Bizible和其他Adobe Experience Cloud应用程序之间创建一致的体验。

* **Bizible域所有权和自我管理**:Bizible用户可以利用Adobe Admin Console管理他们希望Bizible跟踪的域。这为以前的手动流程提供了自助服务，并在如何跨Adobe Experience Cloud应用程序管理域所有权和跟踪方面提供了一致的体验。

## 公告 {#announcements}

* **更新了订阅通用ID设置**:为支持即将面向现有用户的Marketo Engage和Adobe身份集成，所有Marketo Engage订阅都将在启用通用ID支持时统一进行。
