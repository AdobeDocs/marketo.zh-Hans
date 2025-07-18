---
unique-page-id: 13795395
description: 发行说明 — 2018年冬季 — Marketo文档 — 产品文档
title: 发行说明 — 2018年冬季
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 发行说明： 2018年冬季 {#release-notes-winter}

’18年冬季版本包括以下功能。 检查您的Marketo版本以了解功能可用性。

请单击标题链接以查看每个功能的详细文章。 **注意**：此版本中包含的某些功能没有关联的文章。 如果一个主题有多个子标题，则链接会放置在该处。

## Campaign性能和吞吐量增强 {#campaign-performance-and-throughput-enhancements}

Marketo正在利用我们的大数据架构提高触发活动吞吐量和改进Web活动处理，以使您可更快地响应受众的操作。

## Marketo [!DNL Salesforce] CRM集成的增强功能 {#enhancements-to-marketo-s-salesforce-crm-integration}

我们对[!DNL Salesforce] CRM集成进行了两项增强：

* 针对某些CRM同步失败（凭据已过期、达到API限制等），[Marketo管理员通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)

* [能够在潜在客户分配时关闭向潜在客户所有者的电子邮件通知](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md)

这些改进将在2018年推出。

## [Marketo性能分析](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>[!UICONTROL Performance Insights]是附加产品。 请联系您的Marketo客户成功经理或客户经理以获取报价。

利用归因分析、交互式可视化图表和详细的数据表，探索您的营销活动和渠道如何影响业务成果。

![](assets/image2018-2-5-7-3a55-3a46.png)

## 基于帐户的营销增强功能 {#account-based-marketing-enhancements}

**[ABM层次结构](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

对于具有[!DNL Salesforce]或[!DNL Microsoft Dynamics]的ABM客户，ABM现在将自动继承（和显示）在CRM中建立的父子关系。 您将能够在汇总报告和活动执行中使用这些关系。

## 电子邮件营销 {#email-marketing}

**[动态电子邮件脚本](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

现在，使用动态内容的电子邮件支持Velocity脚本。 将速度与基于分段的动态内容相结合，创建高度个性化的电子邮件。

**收件人时区**

* **[每月培养节奏](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**：我们添加了每月安排培养计划的功能。

* **[停止投放](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**：您现在可以停止运行期间剩余的任何发送。

## 广告网络集成 {#ad-network-integrations}

**[Google客户匹配集成](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

利用此集成，您可以将Marketo受众发送到Google以使用[!DNL Google AdWords]进行定位，以及跨[!DNL YouTube]、Search和[!DNL Gmail]重新定位受众。

**[[!DNL LinkedIn] 匹配的受众API增强功能](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

现在，我们新的[!DNL LinkedIn] API允许您跨多个[!DNL LinkedIn] Campaign Manager帐户重新定位Marketo数据库中的人员。

## Web Personalization {#web-personalization}

适用于Web Personalization的&#x200B;**日语数据Source**

Marketo正在为Web Personalization添加另一个日本数据源，以改进来自日本的访客的Web访客识别（反向IP查找）和个性化。 组织名称将以日语显示。

**[使用静态列表创建Web区段](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization现在可以为已知的Web访客个性化内容，该访客属于营销活动(MLM)中定义的静态列表。 借助此增强功能，您现在可以跨渠道向静态列表进行营销，并通过网站上的个性化内容定位这些列表上的人员。

## 内容人工智能 {#contentai}

**预测算法改进**

通过Marketo优化的ContentAI算法推荐的内容生成的点击次数是随机内容的两倍。

## 集成 {#integration}

**[激活/停用营销活动API](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**

此新API允许您远程激活和取消激活触发器营销活动，因此您现在可以创建完全自动化的项目模板。 只需创建一次项目模板，即可自动执行克隆、营销宣传材料更新，现在即可激活/计划智能营销活动。

## [!DNL ToutApp] {#toutapp}

**取消订阅更新**

从2018年3月1日开始，从[ToutApp.com](https://ToutApp.com)（并使用[!DNL Salesforce]中的“带有[!DNL Tout]的电子邮件”按钮）发送的所有电子邮件都将有一个取消订阅链接附加到底部。

**实时信息源更新**

我们更新了“参与”和“任务”选项卡的外观，使销售成员能够更快、更轻松地直接从实时信息源响应其客户的活动。

**人员详细信息视图更新**

改进的人员详细信息视图(PDV)通过汇总您的[!DNL Tout]和[!DNL Salesforce] CRM联系人详细信息提供了您联系人的全面视图。
