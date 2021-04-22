---
unique-page-id: 2360370
description: 如何在同步之前匹配项目状态和Salesforce活动状态 — Marketo文档 — 产品文档
title: 如何在同步之前匹配项目状态和Salesforce活动状态
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 如何在同步之前匹配项目状态和Salesforce活动状态{#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

本文介绍如何修复不兼容的状态错误并映射Marketo项目和Salesforce活动同步之前的状态。

## 如果收到错误消息{#what-do-you-do-if-you-received-an-error-message}，该怎么办

如果您尝试同步到包含潜在客户的现有Salesforce活动，而该活动包含一个或多个不兼容状态，则会显示一条错误消息。 如果状态不是完全匹配，则Marketo项目和Salesforce活动&#x200B;*将不会*&#x200B;同步。

![](assets/image2015-7-22-9-3a23-3a29.png)

从此错误消息中，您可以选择：

1. 从下拉菜单或
1. 您可以取消，修复状态错误，并在修复错误后尝试同步。 要修复状态错误，请执行以下操作之一：

   * 登录Salesforce并删除或重命名不兼容的活动成员状态，以映射到用于与您的Marketo项目关联的渠道类型的Marketo项目状态。
   * 在Marketo中修改项目状态，以映射到您的Salesforce活动成员状态。 这是Marketo Admin功能。 有关详细信息，请参阅[创建项目渠道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)。
