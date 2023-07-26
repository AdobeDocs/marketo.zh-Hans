---
unique-page-id: 1147328
description: 电子邮件中的硬退信和软退信 — Marketo文档 — 产品文档
title: 电子邮件中的硬退信和软退信
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 电子邮件中的硬退信和软退信 {#hard-and-soft-bounces-in-email}

当邮件服务器通知Marketo无法传递某人的电子邮件时，硬退回可能会导致该人的电子邮件地址无效。 软退回意味着将电子邮件交付给人员时出现问题；此问题会自动解决，有时可能需要几天。 硬退信和软退信都包括 [多个类别](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## 退回分类 {#bounce-classification}

Marketo中有5个人员字符串与存在问题的电子邮件投放相关。

1. **电子邮件已暂停**  — 在发生特定类型的硬退回时，设置为True。
1. **电子邮件暂停原因**  — 原因有很多。 此字段试图解释原因。
1. **电子邮件暂停时间**  — 发生违规退回时，Marketo将暂停从该时间戳中向此人发送邮件24小时。
1. **电子邮件无效**  — 在发生特定类型的硬退回时，设置为True。
1. **电子邮件无效原因**  — 硬退回的原因。

>[!NOTE]
>
>人员到达 **电子邮件已暂停** 状态，无法清除电子邮件已暂停复选框。 然而，该人仍将在最初被停职后24小时被邮寄。
>
>当人员标记为 **电子邮件无效**，则只能通过取消选中其记录的“人员信息”选项卡中的“电子邮件无效”框来手动重置电子邮件（我们建议您仅在您知道其电子邮件有效时才手动重置）。

>[!PREREQUISITES]
>
>关注 [这些步骤](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) 创建电子邮件性能报表，以生成退回数据。

创建电子邮件性能报表后，屏幕应如下所示：

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾邮件过滤器有时会产生硬退回。 这些“误报”并不表明此人电子邮件地址的真实有效性。
