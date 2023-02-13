---
description: 发行说明 — 2022年1月 — Marketo文档 — 产品文档
title: 发行说明 — 2022年1月
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: ec783ee58e3c249da036d4770231eb9d7ef61bbd
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 发行说明：2022年1月 {#release-notes-jan-22}

’22年1月版中包含以下功能。 查看您的Adobe Marketo Engage版本以了解功能的可用性。

>[!AVAILABILITY]
>
>由星(![星星](assets/yellow-star.png))是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_**

将在 **2022年1月21日**，在接下来的几周内（除非另有指定）分阶段推出每项功能。

## 新一代体验 {#modern-ux}

* **更新了下一代体验中的屏幕**:我们将在下一代体验中提供额外的刷新屏幕，这些屏幕提供了可通过切换开关访问的更新设计和可用性增强功能：

   * Design Studio中的登陆页面资产详细信息
   * 营销活动中的登陆页面资产详细信息

## Microsoft Dynamics集成 {#microsoft-dynamics-integration}

* **正在同步多选选项集字段类型通常可用**:从Microsoft Dynamics中同步多选选项集字段类型，以便在智能列表和智能营销活动中利用该字段类型，以实现更精细的受众定位。 示例包括：感兴趣的主题/产品、首选的通信模式等。 此新同步适用于Microsoft Dynamics版本9.X（包括Dynamics 365 Online）。

* **Microsoft Dynamics 365 Online的服务器到服务器身份验证**:为了提高安全性，我们现在将支持服务器到服务器(S2S)，作为Azure Active Directory上Marketo Engage同步用户的额外身份验证模式，以便非交互式访问Microsoft Dynamics 365 Online。 这允许您采用多重身份验证，因为所有身份验证和登录都将基于OAuth（仅客户端ID和客户端密钥）。

>[!NOTE]
>
>S2S模式基于应用程序用户，而不是授权用户，这样可以节省额外许可证的使用。

## 管理 {#administration}

* **[表单验证规则](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**:维护数据库的运行状况，能够阻止有问题或不希望的电子邮件域提交Marketo Engage表。 全局表单验证规则面板允许管理员定阻止列表义，或启用预定义的自由使用者域列表以阻止表单。

* **[登陆页面标题安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**:管理员可以在其登陆页面域上管理严格传输安全和X-Frame选项标头，以强制执行强大的安全要求。

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

## AEPMarketo Engage目标连接器 — 创建新潜在客户 {#aep-marketo-engage-destination-connector}

同时使用Adobe Experience Platform(AEP)的Marketo Engage客户可以通过AEP目标连接器将新人员记录从AEP推送到Marketo Engage，从而最大限度地提升其数据库。 将受众区段从AEP发送到Marketo Engage时，区段中不存在于Marketo Engage数据库中的人员 [可以自动添加到其中](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## 销售分析 {#sales-insight}

![（星号）](assets/yellow-star.png)

**适用于Salesforce CRM的Sales Insight**

* **新类型列以获得最佳结果**:在“最佳下注”页面上，卖家将通过标有“类型”的新列来区分潜在客户和联系人，从而更快地获得洞察信息。

* **Salesforce平台API更新**:为响应Salesforce停用的Salesforce平台API版本21.0至30.0，已使用最新API更新Sales Insight包。

* **更新了品牌策略**:所有销售分析页面都将进行更新，以便与Adobe品牌保持一致。

**Microsoft Dynamics的销售分析**

* **更新了帐户布局**:卖家可以集体查看排名最前的活动，例如：帐户内所有联系人的电子邮件活动、web活动、有趣时刻和分数变化。

## Sales Connect {#sales-connect}

![（星号）](assets/yellow-star.png)

* **调用结果和原因**:使用完全可自定义的新呼叫结果和呼叫原因选项，更加详细地了解和跟踪销售团队的出站工作。 除了这些新字段外，我们还引入了新的管理功能，以在销售者进行呼叫时强制执行呼叫原因和结果选择，新的管理功能用于启用或禁用呼叫原因和结果，以及新的呼叫原因和呼叫结果Salesforce活动自定义字段，用于将数据记录到Salesforce。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) 以了解更多。

* **Salesforce活动详细信息自定义**:通过自定义在销售活动从Sales Connect记录到Salesforce时将哪些信息添加到Salesforce任务主题字段，在Salesforce中捕获更多销售活动和任务数据。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) 以了解更多。

## 公告 {#announcements}

* **Marketo Sky弃用**:今年3月，由于我们将资源集中在提供下一代用户体验上，因此Marketo Sky将不再可用。 为了保持对当今Marketo Sky所独有的功能的访问，我们将在3月将资产到期和智能促销活动优先级覆盖引入主流体验。 [单击此处](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) 以了解更多。

* **弃用表单端点**:指向leadCapture/save2端点的不支持的程序化表单POST将被Marketo Engage表单拒绝。 [单击此处](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) 以了解更多。

**Marketo Engage域 — Sales Insight配置**:对于未设置SSL证书的Marketo Engage域和https://，调用将失败，并出现SSL握手错误。 因此，这些领域将被废除。 因此，如果Sales Insight用户具有指向其中任何域的旧配置，则他们的潜在客户、联系人、帐户、机会面板或Marketo全局页面上可能会出现系统标注错误。 我们建议您更新 [Marketo Engage配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) 在Salesforce中遇到此错误时，不会将其标记为“隐藏”。 您只需更新文档“Marketo销售分析配置”部分中突出显示的Marketo Engage凭据。

**_产品发行网络研讨会_**

[2022年1月版Marketo Engage网络研讨会](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
