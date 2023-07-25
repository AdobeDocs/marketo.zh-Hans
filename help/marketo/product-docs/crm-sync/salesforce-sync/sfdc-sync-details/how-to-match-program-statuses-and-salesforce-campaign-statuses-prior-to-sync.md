---
unique-page-id: 2360370
description: 如何在同步之前匹配项目状态和Salesforce Campaign状态 — Marketo文档 — 产品文档
title: 如何在同步之前匹配项目状态和Salesforce Campaign状态
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 如何在同步之前匹配项目状态和Salesforce Campaign状态 {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

本文介绍了如何修复不兼容的状态错误，并在Marketo程序和Salesforce Campaign同步之前映射状态。

## 如果收到错误信息，该怎么办 {#what-do-you-do-if-you-received-an-error-message}

如果尝试同步到包含潜在客户的现有Salesforce营销活动，并且该营销活动包含一个或多个不兼容的状态，则会显示错误消息。 Marketo项目和Salesforce营销活动 *不会* 如果状态不是完全匹配则同步。

![](assets/image2015-7-22-9-3a23-3a29.png)

从该错误消息中，您可以选择执行以下操作：

1. 从下拉菜单中选择要同步到的其他营销活动，或者
1. 您可以取消、修复状态错误并在修复错误后尝试同步。 要修复状态错误，请执行下列操作之一：

   * 登录Salesforce，删除或重命名不兼容的Campaign成员状态，以映射到与您的Marketo项目关联的渠道类型所使用的Marketo项目状态。
   * 修改Marketo中的项目状态，以映射到您现有的Salesforce促销活动成员状态。 这是Marketo管理功能。 有关详细信息，请参阅 [创建项目群渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
