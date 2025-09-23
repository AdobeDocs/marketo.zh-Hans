---
unique-page-id: 2951044
description: 发行说明 — 2014年5月 — Marketo文档 — 产品文档
title: 发行说明 — 2014年5月
exl-id: c7b5b2c1-ea3d-483b-8a65-c4d6313bfe31
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# 发行说明：2014 年 5 月 {#release-notes-may}

2014年5月版本中包含以下功能。 请检查您的Marketo版本以了解功能可用性。 发布后，请务必返回以查找每个功能的详细知识库文章的链接！

## 删除Workspace {#delete-workspace}

现在您可以[删除未使用的工作区](/help/marketo/product-docs/administration/workspaces-and-person-partitions/delete-a-workspace.md)。 在尝试删除工作区之前，请确保将所有资源移动到另一个工作区。

## 安排首次点播 {#schedule-first-cast}

在参与程序中，您可以安排[首次播放运行](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)的日期。 例如，指定每2周播放一次，然后选择第一次播放的日期。

![](assets/image2014-9-22-11-3a57-3a36.png)

![](assets/image2014-9-22-11-3a57-3a54.png)

## 增强参与计划 {#enhanced-engagement-programs}

现在，每个人都拥有多个程序、流和通信限制。

## 文本电子邮件中的链接跟踪 {#link-tracking-in-text-emails}

[在电子邮件文本版本的URL两侧添加双方括号](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-tracked-links-to-a-text-email.md)，以指示何时应将链接转换为重定向的Marketo跟踪链接

>[!NOTE]
>
>**示例**
>
>`[[https://www.marketo.com]]`

默认情况下，电子邮件文本版本中不会跟踪任何链接。 添加此新语法以指示何时应将链接转换为跟踪链接。 HTML链接的行为未更改。  要在电子邮件中添加跟踪链接，请执行以下操作：

* **HTML版本：**&#x200B;只需插入您的链接即可。 默认情况下，将对其进行跟踪。
* **文本版本：**&#x200B;输入由双方括号括起的URL。

要在电子邮件中添加未跟踪的链接，请执行以下操作：

* **HTML版本：**&#x200B;插入您的链接并将“mktNoTrack”类添加到该链接中。
* **文本版本：**&#x200B;只需输入URL即可。 默认情况下，将取消跟踪该活动。

![](assets/image2014-9-22-12-3a1-3a34.png)

## 示例电子邮件中的链接标记 {#link-markup-in-sample-emails}

提前查看您的链接在电子邮件中的行为方式。 现在，示例电子邮件会显示这些链接在潜在客户面前的确切显示方式。 预览哪些链接已转换为跟踪链接，以便您更好地了解消息实际显示给收件人的方式。

## [!UICONTROL Abort Campaign] {#abort-campaign}

不要惊慌！ 如果发现错误，请使用新的[中止营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)按钮立即停止其跟踪的营销活动。 您将收到一条通知，其中概述了营销策划停止时每个流程步骤中待定的潜在客户数量。

## [!UICONTROL Sales Insight]日语、葡萄牙语和西班牙语 {#sales-insight-in-japanese-portuguese-and-spanish}

从AppExchange下载[!UICONTROL Sales Insight]的最新版本，以便您的日语、葡萄牙语和西班牙语销售代理使用其首选语言查看[!UICONTROL Sales Insight]内容。

![](assets/image2014-9-22-12-3a2-3a12.png)

## 计划会员资格分析中的计划状态和成功时间范围 {#program-status-and-success-timeframe-in-program-membership-analysis}

查看每个计划状态[中有多少](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/build-a-program-membership-analysis-report-that-lists-leads.md)成员，以及他们更改为每个状态的时间，包括他们获得计划成功的日期。

## [!UICONTROL Email Analysis]中的A/B测试电子邮件 {#a-b-test-emails-in-email-analysis}

在[中报告每个](/help/marketo/product-docs/reporting/revenue-cycle-analytics/email-analysis/build-an-email-analysis-report-that-shows-program-information.md)A/B测试电子邮件变体[!UICONTROL Email Analysis]。

## Analytics打包更改 {#analytics-packaging-changes}

Revenue Cycle Modeler和Success Path Analyzer现在包含在MA标准版中。

## 移动平台信息 {#mobile-platform-info}

[细分并触发](/help/marketo/product-docs/reporting/basic-reporting/report-activity/build-a-people-performance-report-with-mobile-platform-columns.md)潜在客户打开和单击其移动设备的电子邮件。
