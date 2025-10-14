---
unique-page-id: 11384018
description: 发行说明 — 2016年秋季 — Marketo文档 — 产品文档
title: 发行说明 — 2016年秋季
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# 发行说明：2016 年秋季 {#release-notes-fall}

2016年秋季版本中包含以下功能。 检查您的Marketo版本以了解功能可用性。 请单击标题链接以查看每个功能的详细文章。

## 电子邮件中的[!UICONTROL Predictive Content] {#predictive-content-in-email}

我们的[!UICONTROL Predictive Content]应用程序现在有了新的用户体验，可以通过我们的机器学习和预测算法跨Web和电子邮件渠道跟踪、管理和推荐您的内容。

>[!NOTE]
>
>所有使用预测模块的客户将于1月10日前启用。

![](assets/shafe.png)

您现在可以向电子邮件添加预测性内容。 打开电子邮件时，收件人会自动收到相关的推荐内容，这有助于提高内容参与度和转化率。

![](assets/predictive.png)

## [Facebook离线转化](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

通过[!DNL Facebook]离线转化集成，Marketo中的转化数据（适用于潜在广告商机）会自动发送回[!DNL Facebook]，以便您的广告团队可以更好地优化其广告支出。 在此[!DNL Facebook]广告管理器报表中，脱机转化突出显示。

![](assets/facebook.png)

## [通用ID](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

通用ID允许您通过一次登录访问多个Marketo订阅，并快速在订阅之间切换。 您可以将单个社区配置文件用于所有订阅。

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>请联系Marketo支持以启用此功能。

## 基于Marketo帐户的营销增强功能 {#marketo-account-based-marketing-enhancements}

现在，您可以将帐户团队分配给基于帐户的营销(ABM)中的指定帐户，例如帐户所有者、销售开发代表、业务开发代表和客户成功经理。 您还可以构建特定于帐户所有者的帐户列表，并向帐户团队发送个性化的每周ABM报告。

![](assets/account-team-11-15-16.png)

**REST API**

此版本还允许您使用Marketo REST API在ABM中管理指定帐户属性和帐户分数。 有关API操作的更多详细信息，请访问[Marketo开发人员网站](https://developers.marketo.com/rest-api/lead-database/named-accounts)。

## [审核记录增强功能](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

审核记录提供了Marketo订购中所做更改的全面历史记录。 我们为项目添加了其他跟踪功能，并展示了智能营销活动、智能列表以及对用户和角色所做更改的重要更改详细信息。

## 新权限

**使电子邮件正常工作**

以前，您必须担心用户向数据库中已取消订阅的用户发送事务性电子邮件，现在这种日子已经一去不复返了。 您现在可以指定哪些用户可以使电子邮件成为可操作电子邮件或编辑操作电子邮件。

**编辑营销活动限制**

如果无法强制执行[营销活动限制](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md)，为什么要设置这些限制？ 当您将营销活动限制设置设置为限制数据库中可通过单个营销活动进行定位的人员数量时，您现在能够限制哪些用户在计划营销活动时可以覆盖这些设置。

## [移动推送通知的声音](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

通过启用声音功能，为您的iOS推送通知增添丰富内容。 这项新功能允许您在移动设备上显示推送通知时触发声音。

>[!NOTE]
>
>* 设备所有者可以选择阻止在设备设置中播放声音，应用程序开发人员可以在应用程序中向设备所有者提供选项来阻止播放声音。
>* 在Android设备上显示推送通知时，会自动播放声音。

![](assets/sound-for-push-notifications.png)

## [与Salesforce Encryption兼容的Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

市场[!DNL Sales Insight]现在与[!DNL Salesforce] Shield Encryption兼容。 所有[!DNL Sales Insight]客户都应升级到此最新的托管包（版本1.4359.2），该包在[&#x200B; [!DNL Appexchange]上有](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO)可用。

## [命名帐户API](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

在此版本中，Marketo ABM用户可以通过指定帐户API管理指定帐户。 用户可以创建、更新和删除指定帐户，也可以读取和更新ABM指定帐户分数。

## [电子邮件编辑器v2.0 API支持](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

使用Marketo REST API管理v2.0格式的电子邮件变量和模块。

## [对Marketo Salesforce Sync的更改](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

Marketo的[!DNL Salesforce]集成正在不断发展，以改进Marketo字段与[!DNL Salesforce]同步的方式。 现在，您无需同步大量您可能需要（也可能不需要）的字段，而是可以选择您要包括的字段。 请在此处查看我们的文档以了解更多信息：[https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840)。
