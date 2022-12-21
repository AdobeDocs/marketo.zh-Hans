---
unique-page-id: 10097199
description: 发行说明 — 2016年冬季 — Marketo文档 — 产品文档
title: 发行说明 — 2016年冬季
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# 发行说明：’16年冬 {#release-notes-winter}

’16年冬季版本中包含以下功能。 请单击标题链接以查看每项功能的详细文章。

## [是匿名过滤器](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

已为智能列表删除“匿名”筛选器。 请参阅 [下一代Munchkin跟踪常见问题解答](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) 文档以了解详细信息。 此更改不会影响Web个性化(RTP),RTP会继续识别匿名和已知的Web访客，并对这些访客实时个性化内容。

## [数据库仪表板](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md) {#database-dashboard}

潜在客户数据库具有更新的摘要功能板，其中包括人员数据库总大小、可销售潜在客户数量以及按前5个来源划分潜在客户。

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Microsoft Edge Browser](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

我们已将Microsoft Edge添加到 [浏览器列表](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) 受Marketo支持。

## [《Microsoft展望2016》](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[《Microsoft展望2016》](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) 现在支持。

## [电子邮件程序开始](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

使用“开始前”指示应提前处理您的发送。 “开始前”不会在计划时间确定潜在客户并准备电子邮件，而是确保这些任务事先完成。 这样，您的受众就会开始在计划时间接收电子邮件。

![](assets/image2016-1-11-15-3a38-3a3.png)

要使用此功能，必须至少提前12小时计划电子邮件程序，并且智能列表将在发送前12小时被锁定。

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>此功能将在’16年冬季版本发布后的一周内逐步推出。 无法与智能营销活动或API一起使用。

## [移动营销增强功能](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**PhoneGap支持：** 现在，我们为您的移动设备应用程序提供PhoneGap支持。 [了解详情](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**支持沙盒应用程序**:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [程序API](https://developers.marketo.com/documentation/programs/) {#program-api}

通过REST API创建、更新和克隆程序。 这不包括在项目中创建或更新智能列表和智能营销策划。

## [Microsoft Dynamics增强功能](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[同步状态](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)**:对同步进程的当前吞吐量和积压工作进行制表。 按插入和更新次数（按对象）划分。

![](assets/pending-backog-cropped.png)

**[通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**:收到常见同步错误的通知，以及存在该错误的潜在客户列表。

![](assets/image2016-1-12-8-3a13-3a9.png)

## [自定义对象增强功能](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

您现在可以使用具有多个链接字段的中间对象，在潜在客户/帐户和自定义对象之间创建多对多关系。

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[Facebook潜在客户广告](https://www.facebook.com/business/a/lead-ads) 是企业在Facebook上运行商机拓展活动的更直接方式。 人们填写表格来表达对产品或服务的兴趣，以便企业可以跟进这些兴趣。 Marketo与Facebook潜在客户广告的集成会自动捕获潜在客户在潜在客户广告表单中提供的信息。 随后可以使用新的“填充Facebook潜在客户广告”触发器自动执行后续操作和通知。

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Web（实时个性化）促销活动计划程序](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

提前计划营销活动。 设置个性化Web内容的开始和结束日期，并在特定日期和时间重复营销活动。 根据Web访客的时间或选定的时区个性化计划以显示营销活动。

![](assets/image2016-1-14-8-3a36-3a36.png)
