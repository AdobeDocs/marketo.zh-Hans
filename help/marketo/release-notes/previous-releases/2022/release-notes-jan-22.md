---
description: 发行说明 — 2022年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2022年1月
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 发行说明： 2022年1月 {#release-notes-jan-22}

2022年1月版中包含以下功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号(![星形](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

以下功能将开始发布 **2022年1月21日**，在接下来的几周内分阶段推出每个功能（除非另有说明）。

## 新一代体验 {#modern-ux}

* **更新了新一代体验中的Screens**：我们将在下一代体验中提供额外的刷新屏幕，这些屏幕提供更新的设计和可用性增强功能，可通过切换开关访问：

   * Design Studio中的登陆页面资产详细信息
   * 营销活动中的登陆页面资产详细信息

## Microsoft Dynamics集成 {#microsoft-dynamics-integration}

* **多选选项集字段类型同步功能一般可用**：同步Microsoft Dynamics中的多选选项集字段类型，以便在智能列表和智能营销活动中使用，以实现更精细的受众定位。 示例包括：主题/感兴趣的产品、首选通信模式等。 此新同步可用于Microsoft Dynamics版本9.X（包括Dynamics 365 Online）。

* **用于Microsoft Dynamics 365 Online的服务器到服务器身份验证**：为了提高安全性，我们现在将支持Server to Server (S2S)作为Azure Active Directory上的Marketo Engage同步用户的附加身份验证模式，以便以非交互方式访问Microsoft Dynamics 365 Online。 这允许您采用多重身份验证，因为所有身份验证和登录都将基于OAuth（仅客户端ID和客户端密码）。

>[!NOTE]
>
>S2S模式基于“应用程序用户”而非“许可用户”，这节省了使用额外的许可证。

## 管理 {#administration}

* **[表单验证规则](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：维护数据库的运行状况，能够阻止有问题或不需要的电子邮件域提交Marketo Engage表单。 “全局表单验证规则”面板允许管理员定义阻止列表或启用要阻止表单的免费使用者域的预定义列表。

* **[登陆页面页眉安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理员可以管理其登陆页面域上的严格传输安全和X-Frame Options标头，以强制实施严格的安全要求。

**_将在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## AEPMarketo Engage目标连接器 — 创建全新潜在客户 {#aep-marketo-engage-destination-connector}

同时使用Adobe Experience Platform (AEP)的Marketo Engage客户可以最大限度地利用其数据库，通过AEP目标连接器将全新人员记录从AEP推送到Marketo Engage中。 将受众区段从AEP发送到Marketo Engage时，区段内尚不存在于Marketo Engage数据库中的人员 [可以自动添加到其中](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## 销售分析 {#sales-insight}

![(star)](assets/yellow-star.png)

**Sales Insight for Salesforce CRM**

* **最佳匹配的新类型列**：通过“最佳匹配”页面上标记为“类型”的新列来区分潜在客户和联系人，销售人员将更快地获得洞察。

* **Salesforce平台API更新**：为响应Salesforce弃用Salesforce平台API版本21.0到30.0 ，已使用最新的API更新了Sales Insight包。

* **更新的品牌**：正在更新所有Sales Insight页面，以与Adobe品牌保持一致。

**Microsoft Dynamics的销售分析**

* **已更新帐户布局**：卖家可以获得热门活动的集体视图，例如：电子邮件活动、Web活动、有趣的时刻，以及帐户中所有联系人的得分变化。

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **致电结果和原因**：通过新的、完全可自定义的致电结果和致电原因选项，更详细地了解和跟踪销售团队的出站工作。 除了这些新字段之外，我们还引入了新的治理机制，以便在销售商进行呼叫时强制实施呼叫原因和结果选择；引入了新的治理机制，以便启用或禁用呼叫原因和结果；还引入了新的呼叫原因和呼叫结果Salesforce活动自定义字段，以便将数据记录到Salesforce。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) 了解更多信息。

* **Salesforce活动详细信息自定义**：当销售活动从Sales Connect记录到Salesforce中时，通过自定义添加到Salesforce任务主题字段中的信息，在Salesforce中捕获更多销售活动和任务数据。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) 了解更多信息。

## 公告 {#announcements}

* **Marketo Sky弃用**：三月份，我们将不再提供Marketo Sky，因为我们的资源致力于提供新一代用户体验。 为了保持对当前独有的Marketo Sky功能的访问，我们在3月份将资产到期和智能营销活动优先级覆盖引入主流体验。 [单击此处](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) 了解更多信息。

* **表单端点弃用**：Marketo Engage表单将拒绝不支持的对leadCapture/save2端点的编程表单POST。 [单击此处](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) 了解更多信息。

**Marketo Engage域 — Sales Insight配置**：对于未配置SSL证书和https://的Marketo Engage域，调用将失败，并出现SSL握手错误。 因此，这些领域将会被淘汰。 因此，如果配置较旧的Sales Insight用户指向其中的任何域，则他们的Lead 、 Contact 、 Account 、 Opportunity Panels或Marketo Global页面上可能会出现系统标注错误。 我们建议您更新 [Marketo Engage配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 如果您遇到此错误，请使用Salesforce。 您只需更新文档中突出显示“Marketo销售分析配置”部分的Marketo Engage凭据即可。

**_产品发布网络研讨会_**

[2022年1月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
