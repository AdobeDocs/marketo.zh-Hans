---
unique-page-id: 1147091
description: 了解计划会员资格 — Marketo文档 — 产品文档
title: 了解计划会员资格
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
source-git-commit: 66baa78d3e32140526d8d66beba493e02937a2c2
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 了解计划会员资格 {#understanding-program-membership}

>[!NOTE]
>
>Marketo现在正在对所有订阅实施语言标准化，因此您可能会在订阅中看到商机/商机，并在docs.marketo.com中看到个人/人员。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他的变化。 [了解更多](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**定义：** 成员是在项目中具有状态的人员。

## 人如何成为项目成员 {#how-people-become-members-of-a-program}

1. 人填写 [登陆页面上的表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) 在程序中。

   1. 人员将自动具有进度中的第一个状态。

1. 您 [将成员导入程序](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) 文件。

   1. 人员将自动具有进度中的第一个状态。

1. 您使用 [更改程序状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) 流步骤。
1. 个人注册或参加 [网络研讨会与活动项目同步](/help/marketo/product-docs/demand-generation/events/events/event-partners.md).
1. 人是 [使用Marketo iPad签入应用程序创建](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. 将人员添加到SFDC营销活动，即 [同步到程序](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>对于电子邮件程序，仅当发送电子邮件时，才会将人员添加到会员资格中。

## 项目状态 {#program-statuses}

项目状态是指用户在项目中完成的步骤（例如，已邀请、已回复、已出席、无节目）。 这些步骤由 [频道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>人员无法向后移动到早期程序状态。 状态进度只是一种方式。

## 成功状态 {#success-statuses}

项目的目的是与人员或潜在客户进行有意义的互动。 当人员达到达到该目标的状态时，即表示成功。

>[!NOTE]
>
>对于网络研讨会，如果实际不观看网络研讨会，则注册并不是有意义的交互。 在这种情况下，参加是成功的。

## 客户获取计划  {#acquisition-program}

当新名称以程序成员身份进入系统时，Marketo会自动将该程序设置为“获取”。 这为 [首次联系归因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [在项目中使用标记](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [创建项目绩效报告](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

