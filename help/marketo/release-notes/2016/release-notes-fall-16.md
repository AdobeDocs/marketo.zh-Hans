---
unique-page-id: 11384018
description: 发行说明 — ’16年秋季 — Marketo文档 — 产品文档
title: 发行说明 — 1916年秋季
exl-id: da935951-162e-426c-acf2-12c55ff706b4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 发行说明：’16年秋{#release-notes-fall}

’16年秋季版包含以下功能。 查看您的Marketo版本以了解功能可用性。 请单击标题链接，以视图每种功能的详细文章。

## 电子邮件{#predictive-content-in-email}中的预测内容

我们的预测内容应用程序提供了全新的用户体验，可通过我们的机器学习和预测算法在Web和电子邮件渠道中跟踪、管理和推荐您的内容。

>[!NOTE]
>
>在1月10日之前，所有具有预测模块的客户都将启用。

![](assets/shafe.png)

您现在可以向电子邮件中添加预测性内容。 打开电子邮件时，收件人会自动接收相关的推荐内容，从而帮助提高内容参与度和转化率。

![](assets/predictive.png)

## [Facebook Offline Conversions](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

通过Facebook Offline Conversions集成，Marketo（针对潜在客户广告潜在客户）中的转化数据将自动发送回Facebook，以便您的广告团队能够更好地优化其广告支出。 在此Facebook Ad Manager报表中，将高亮显示脱机转换。

![](assets/facebook.png)

## [通用ID](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

通用ID允许您通过一次登录访问多个Marketo订阅，并在订阅之间快速切换。 您可以对所有订阅使用单一社区用户档案。

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>请联系Marketo支持以启用此功能。

## Marketo基于帐户的营销增强{#marketo-account-based-marketing-enhancements}

现在，您可以在“基于帐户的营销”(ABM)中将帐户团队分配给指定帐户，例如，帐户所有者、销售发展代表、业务发展代表和客户成功经理。 您还可以构建特定于帐户所有者的帐户列表，并向帐户团队发送个性化的每周ABM报告。

![](assets/account-team-11-15-16.png)

**REST API**

此版本还允许您使用Marketo REST API在ABM中管理命名帐户属性和帐户分数。 有关API操作的详细信息，请访问[Marketo Developers网站](https://developers.marketo.com/rest-api/lead-database/named-accounts)。

## [审计线索增强](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

审计跟踪提供了在Marketo订阅中所做更改的完整历史记录。 我们为项目添加了额外的跟踪功能，并为智能活动、智能列表以及对用户和角色所做的更改提供了重要的更改详细信息。

## [新权限](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**使电子邮件可操作**

不得不担心用户向数据库中取消订阅的用户发送交易电子邮件的日子已经一去不复返。 您现在可以指定哪些用户可以使电子邮件正常工作或编辑操作电子邮件。

**编辑活动限制**

如果您无法强制执行[活动限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md)，为何要设置这些限制？ 在设置“活动限制设置”以限制数据库中可以使用单个活动定位的人员数量时，您现在可以限制哪些用户在计划活动时可以覆盖这些设置。

## [移动推送通知的声音](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

通过启用声音，为iOS推送通知增添丰富性。 此新功能允许您在移动设备上显示推送通知时触发声音。

>[!NOTE]
>
>* 设备所有者可以选择阻止在设备设置中播放声音，应用程序开发人员可以在应用程序中为设备所有者提供选项以防止播放声音。
>* 当Android设备上显示推送通知时，会自动播放声音。


![](assets/sound-for-push-notifications.png)

## [与Salesforce加密兼容的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight现在与Salesforce Shield Encryption兼容。 所有Sales Insight客户应升级到此最新的受管程序包（版本1.4359.2），该程序包[可在Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO)上找到。

## [指定帐户API](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

在此版本中，Marketo ABM用户可以通过指定帐户API管理指定帐户。 用户可以创建、更新和删除指定帐户，并读取和更新ABM指定帐户得分。

## [电子邮件编辑器v2.0 API支持](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

使用Marketo REST API以v2.0格式管理电子邮件的变量和模块。

## [对Marketo Salesforce同步的更改](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

Marketo的Salesforce集成正在不断发展，以改进Marketo字段与Salesforce同步的方式。 现在，您无需同步可能需要或可能不需要的大量字段，而是可以选择要包含的字段。 有关更多信息，请单击此处查阅我们的文档：[https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840)。
