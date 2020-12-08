---
unique-page-id: 11384018
description: 发行说明-2016年秋季版- Marketo文档——产品文档
title: 发行说明- 1916年秋季版本
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---


# 发行说明：1916年秋 {#release-notes-fall}

1916年秋季版本包含以下功能。 检查您的Marketo版本以了解功能可用性。 请单击标题链接，以视图每个功能的详细文章。

## [电子邮件中的预测内容](http://docs.marketo.com/display/docs/predictive+content)  {#predictive-content-in-email}

我们的预测内容应用程序具有新的用户体验，可通过我们的机器学习和预测算法在Web和电子邮件渠道中跟踪、管理和推荐您的内容。

>[!NOTE]
>
>在1月10日之前，所有使用预测模块的客户都将启用该功能。

![](assets/shafe.png)

您现在可以向电子邮件中添加预测性内容。 打开电子邮件时，收件人会自动收到相关的推荐内容，从而帮助提高内容参与度和转化率。

![](assets/predictive.png)

## [Facebook脱机转换](../../product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)  {#facebook-offline-conversions}

通过Facebook脱机转化集成，Marketo中的转化数据（针对潜在客户广告潜在客户）会自动发送回Facebook，以便您的广告团队能够更好地优化其广告支出。 在此Facebook广告管理器报告中，将突出显示脱机转换。

![](assets/facebook.png)

## [通用ID](../../product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

通用ID允许您通过一次登录访问多个Marketo订阅并在订阅之间快速切换。 您可以对所有订阅使用单一社区用户档案。

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>请联系Marketo支持以启用此功能。

## [基于Marketo帐户的营销增强功能](http://docs.marketo.com/pages/viewpage.action?pageid=11380718) {#marketo-account-based-marketing-enhancements}

现在，您可以在“基于帐户的营销”(ABM)中将客户团队分配给指定帐户，例如，帐户所有者、销售开发代表、业务开发代表和客户成功经理。 您还可以构建特定于帐户所有者的帐户列表，并向帐户团队发送个性化的每周ABM报告。

![](assets/account-team-11-15-16.png)

**REST API**

此版本还允许您使用Marketo REST API在ABM中管理命名帐户属性和帐户得分。 有关API操作的更多详细信息，请访 [问Marketo开发人员网站](http://developers.marketo.com/rest-api/lead-database/named-accounts)。

## [审核跟踪增强功能](../../product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

审核跟踪提供了在您的营销订阅中所做更改的完整历史记录。 我们为项目添加了额外的跟踪功能，并为智能活动、智能列表以及对用户和角色所做的更改提供了重要的更改详细信息。

## [新权限](../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**使电子邮件可操作**

您不得不担心用户向数据库中取消订阅的用户发送交易电子邮件的日子已经一去不返。 您现在可以指定哪些用户可以使电子邮件正常工作或编辑操作电子邮件。

**编辑活动限制**

如果无 [法实施活动](http://docs.marketo.com/display/DOCS/Enable+Lead+Restrictions+for+Smart+Campaigns) ，为何要设置这些限制？ 当您设置活动限制设置以限制数据库中可以通过单个活动定位的人员数时，您现在可以限制哪些用户在计划活动时可以覆盖这些设置。

## [移动推送通知声音](../../product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

通过启用声音，为iOS推送通知增添丰富性。 此新增功能允许您在移动设备上显示推送通知时触发声音。

>[!NOTE]
>
>* 设备所有者可以选择阻止在设备设置中播放音效，应用程序开发人员可以在应用程序中为设备所有者提供选项，以阻止播放音效。
>* 在Android设备上显示推送通知时，音效会自动播放。

>



![](assets/sound-for-push-notifications.png)

## [与Salesforce加密兼容的Sales Insight](../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market Sales Insight现在与Salesforce Shield Encryption兼容。 所有Sales Insight客户应升级到最新的托管包（版本1.4359.2），该包可 [在Appexchange上获得](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO)。

## [指定帐户API](http://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

在此版本中，Marketo ABM用户可以通过指定帐户API管理指定帐户。 用户可以创建、更新和删除指定帐户，还可以阅读和更新ABM指定帐户得分。

## [电子邮件编辑器v2.0 API支持](http://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

使用Marketo REST API以v2.0格式管理电子邮件的变量和模块。

## [对Marketo Salesforce同步的更改](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

Marketo的Salesforce集成正在不断改进，以改进Marketo字段与Salesforce同步的方式。 现在，您无需同步可能需要或可能不需要的大量字段，即可选择要包含的字段。 有关更多信息，请单击此处查阅我们的文档： [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840)。

