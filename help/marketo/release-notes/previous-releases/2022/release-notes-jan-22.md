---
description: 发行说明 — 2022年1月 — Marketo文档 — 产品文档
title: 发行说明 - 2022 年 1 月
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# 发行说明： 2022年1月 {#release-notes-jan-22}

2022年1月版中包含以下功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

**_季度发布_**

以下功能将于&#x200B;**2022年1月21日**&#x200B;开始发布，并在接下来的几周内分阶段推出每个功能（除非另有说明）。

## 新一代体验 {#modern-ux}

* **更新了新一代体验中的Screens**：我们将在新一代体验中提供其他更新的屏幕，这些屏幕提供了可通过切换开关访问的最新设计和可用性增强功能：

   * [!UICONTROL Design Studio]中的登陆页面资产详细信息
   * [!UICONTROL Marketing Activities]中的登陆页面资产详细信息

## [!DNL Microsoft Dynamics]集成 {#microsoft-dynamics-integration}

* **多选选项集字段类型的同步功能一般可用**：同步来自[!DNL Microsoft Dynamics]的多选选项集字段类型，以便在智能列表和智能营销活动中利用它们，以实现更精细的受众定位。 示例包括：主题/感兴趣的产品、首选通信模式等。 此新同步可用于[!DNL Microsoft Dynamics]版本9.X（包括Dynamics 365 Online）。

* **用于[!DNL Microsoft Dynamics 365 Online]**&#x200B;的Server to Server身份验证：为了提高安全性，我们现在将支持Server to Server (S2S)作为Azure Active Directory上Marketo Engage同步用户的附加身份验证模式，以便以非交互方式访问[!DNL Microsoft Dynamics 365 Online]。 这允许您采用多重身份验证，因为所有身份验证和登录都将基于OAuth（仅客户端ID和客户端密码）。

>[!NOTE]
>
>S2S模式基于“应用程序用户”而非“许可用户”，这节省了使用额外的许可证。

## 管理 {#administration}

* **[表单验证规则](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**：保持数据库的运行状况，能够阻止有问题或不适当的电子邮件域提交Marketo Engage表单。 “全局表单验证规则”面板允许管理员定义阻止列表或启用要阻止表单的免费使用者域的预定义列表。

* **[登陆页面标头安全性](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**：管理员可以管理其登陆页面域上的严格传输安全性和X-Frame Options标头，以强制实施严格的安全要求。

**_在整个季度中发布_**

以下功能采用非季度周期，并将在未来几个月发布。

## AEP Marketo Engage目标连接器 — 创建全新潜在客户 {#aep-marketo-engage-destination-connector}

同时使用Adobe Experience Platform (AEP)的Marketo Engage客户可以最大限度地利用其数据库，通过AEP目标连接器将全新人员记录从AEP推送到Marketo Engage。 将受众区段从AEP发送到Marketo Engage时，区段中尚不存在于Marketo Engage数据库[中的人员会自动添加到该区段中](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md)。

## [!DNL Sales Insight] {#sales-insight}

![（星形）](assets/yellow-star.png)

**[!DNL Sales Insight]CRM[!DNL Salesforce]的**

* **适用于[!UICONTROL Best Bets]**&#x200B;的新类型列：销售商将通过标记为“类型”的新列快速获得见解，以区分[!UICONTROL Best Bets]页面上的潜在客户和联系人。

* **[!DNL Salesforce]平台API更新**：为响应[!DNL Salesforce]弃用[!DNL Salesforce]平台API版本21.0到30.0，[!DNL Sales Insight]包已更新为最新的API。

* **已更新品牌**：正在更新所有[!DNL Sales Insight]页面，以与Adobe品牌保持一致。

**[!DNL Sales Insight]的[!DNL Microsoft Dynamics]**

* **更新了帐户布局**：销售人员可以获取热门活动的集体视图，例如：电子邮件活动、Web活动、有趣的时刻以及帐户中所有联系人的得分更改。

## [!DNL Sales Connect] {#sales-connect}

![（星形）](assets/yellow-star.png)

* **致电结果和原因**：通过新的、完全自定义的致电结果和致电原因选项，更详细地了解和跟踪您的销售团队的出站努力。 除了这些新字段外，我们还将引入新的治理功能以强制在销售者进行呼叫时选择呼叫原因和结果，引入新的治理功能以启用或禁用呼叫原因和结果，并引入新的呼叫原因和呼叫结果[!DNL Salesforce]活动自定义字段以将数据记录到[!DNL Salesforce]。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812)了解更多信息。

* **[!DNL Salesforce]活动详细信息自定义**：当销售活动从[!DNL Salesforce]登录到[!DNL Salesforce]时，通过自定义添加到[!DNL Salesforce]任务主题字段中的信息，在[!DNL Sales Connect]中捕获更多销售活动和任务数据。 [单击此处](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819)了解更多信息。

## 公告 {#announcements}

* **弃用Marketo Sky**：在3月，Marketo Sky将不再可用，因为我们的资源侧重于提供新一代用户体验。 为了保持对Marketo Sky目前独有的功能的访问权限，我们将在3月份将资产到期和智能营销活动优先级覆盖引入主流体验。 [单击此处](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33)了解更多信息。

* **表单端点弃用**：Marketo Engage表单将拒绝不支持的对leadCapture/save2端点的程序化表单POST。 [单击此处](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631)了解更多信息。

* **在“邀请用户”对话框中登录**：在3月份，将弃用现有的可选“在“邀请用户”对话框中登录”功能。 功能“[!UICONTROL Login in Invite User Dialog]”被通用ID功能覆盖，即将推出的Adobe Identity Management系统集成需要该功能，并且已于2021年8月在所有订阅中启用。 作为弃用的结果，Marketo Engage将强制在订阅中每个电子邮件地址仅关联一个用户。

**Marketo Engage域 — [!DNL Sales Insight]配置**：对于未配置SSL证书和https://的Marketo Engage域，调用将失败，并出现SSL握手错误。 因此，这些领域将会被淘汰。 因此，使用指向这些域中任何域的旧配置的[!DNL Sales Insight]用户可能在其Lead、Contact、Account、Opportunity Panels或Marketo Global页面上遇到系统标注错误。 如果您遇到此错误，我们建议您在[中更新](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)Marketo Engage配置[!DNL Salesforce]。 您只需要更新文档中突出显示“[!DNL Marketo Sales Insight]配置”部分的Marketo Engage凭据。

**_产品发布网络研讨会_**

[2022年1月Marketo Engage发布网络研讨会](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
