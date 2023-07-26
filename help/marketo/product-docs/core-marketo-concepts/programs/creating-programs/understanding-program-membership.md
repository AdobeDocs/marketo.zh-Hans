---
unique-page-id: 1147091
description: 了解计划成员资格 — Marketo文档 — 产品文档
title: 了解计划成员资格
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 了解计划成员资格 {#understanding-program-membership}

>[!NOTE]
>
>Marketo现在正在对所有订阅进行语言标准化，因此您可能会在订阅中看到潜在客户，并在我们的文档中看到相关人员。 这些术语具有相同的含义；它不会影响文章说明。 另外还有一些其它的改变。 [了解详情](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**定义：** 成员是在项目中拥有状态的人员。

## 人员如何成为计划成员 {#how-people-become-members-of-a-program}

1. 用户填写 [登陆页面上的表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) 在程序中。

   1. 人员将自动具有进程中的第一个状态。

1. 您 [将成员导入程序](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) 从CSV文件。

   1. 人员将自动具有进程中的第一个状态。

1. 您使用 [更改项目状态](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) 流程步骤。
1. 人员注册或参加 [与活动项目同步的网络研讨会](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md).
1. 人员是 [使用Marketo iPad签入应用程序创建](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. 向SFDC营销活动添加了一个人员，该人员将 [已同步到项目](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>对于电子邮件计划，仅当发送电子邮件时，才会将人员添加到成员资格。

## 项目状态 {#program-statuses}

计划状态是人们在计划中执行的步骤（例如，已邀请、已回复、已参加、无节目）。 这些步骤由 [渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>人员无法向后移动到较早的计划状态。 状态进程是单向的。

## 成功状态 {#success-statuses}

项目的目的是创建与人员或潜在客户的有意义的交互。 当人员达到达到达到该目标的状态时，将标记成功。

>[!NOTE]
>
>对于网络研讨会，如果注册后未实际观看网络研讨会，则表明注册没有任何意义。 在这种情况下，参与是成功的。

## 客户获取计划  {#acquisition-program}

当新名称作为项目成员进入系统时，Marketo会自动将该项目设置为“客户获取”。 这将建立以下项目的信用 [首次联系归因](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [在项目中使用标记](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [创建计划绩效报表](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)
