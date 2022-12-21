---
unique-page-id: 1147328
description: 电子邮件中的硬退回和软退回 — Marketo文档 — 产品文档
title: 电子邮件中的硬退回和软退回
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 电子邮件中的硬退回和软退回 {#hard-and-soft-bounces-in-email}

当邮件服务器告知Marketo无法发送人员的电子邮件时，硬退回可能会导致人员的电子邮件地址无效。 软退件意味着将电子邮件发送给人时出现问题；这会自动得到解决，有时可能需要数天时间。 硬退回和软退回均由 [多个类别](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## 跳出分类 {#bounce-classification}

Marketo中有5个与问题电子邮件投放相关的人员字符串。

1. **电子邮件已暂停**  — 当发生特定类型的硬退回时，设置为True。
1. **电子邮件挂起原因** 原因有很多。 此字段试图解释原因。
1. **电子邮件暂停于**  — 当出现违规退回时，Marketo将从此时间戳后暂停向该人发送邮件24小时。
1. **电子邮件无效**  — 当发生特定类型的硬退回时，设置为True。
1. **电子邮件无效原因**  — 出现硬反弹的原因。

>[!NOTE]
>
>在人到达 **电子邮件已暂停** 状态时，无法清除电子邮件挂起的复选框。 但是，该人在最初停职后24小时仍然可邮寄。
>
>当某人被标记为 **电子邮件无效**，则只能通过取消选中其记录“人员信息”选项卡中的“电子邮件无效”框来手动重置这些电子邮件（我们建议您仅在知道其电子邮件有效时才重置）。

>[!PREREQUISITES]
>
>关注 [这些步骤](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) 创建电子邮件性能报表，以生成跳出数据。

创建电子邮件性能报表后，屏幕应如下所示：

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾邮件过滤器有时会创建硬退回。 这些“误报”并不表示人员电子邮件地址的真实有效性。
