---
unique-page-id: 1147328
description: 电子邮件中的硬弹回和软弹回- Marketo Docs —— 产品文档
title: 电子邮件中的硬边界和软边界
translation-type: tm+mt
source-git-commit: 615ddd6ffdb3873baa159d440db7b24f3a07e6b0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# 电子邮件中的硬弹回和软弹回{#hard-and-soft-bounces-in-email}

当邮件服务器告知Market该人的电子邮件无法送达时，硬弹回会导致该人的电子邮件地址无效。 软弹跳意味着将电子邮件发送给人时出现问题；这会自动得到解决，有时可能需要数天时间。 硬边界和软边界都由[多个类别](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838)组成。

## 跳出分类{#bounce-classification}

Marketo中有5个与问题电子邮件投放相关的人字符串。

1. **电子邮件已暂停** -当发生某种类型的硬弹回时，设置为“True”。
1. **电子邮件挂起** -原因可能有很多。这个字段试图解释原因。
1. **电子邮件暂停** -发生违规弹回时，Marketo将暂停向该人发送邮件，时间为此时间戳后的24小时。
1. **电子邮件无效** -当发生某种类型的硬弹回时，设置为True。
1. **电子邮件无效** -硬弹回的原因。

>[!NOTE]
>
>当人员达到&#x200B;**电子邮件挂起**&#x200B;状态后，无法清除电子邮件挂起复选框。 不过，在最初停职24小时后，该人仍可邮寄。
>
>当某人被标记为&#x200B;**email invalid**&#x200B;时，只能通过取消选中其记录的“人员信息”选项卡中的“电子邮件无效”框来手动重置他们（我们建议仅在您知道其电子邮件有效时重置）。

>[!PREREQUISITES]
>
>按照[这些步骤](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md)创建电子邮件性能报告，该报告将生成弹回数据。

创建电子邮件性能报告后，屏幕应当如下：

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾邮件过滤器有时会产生硬弹回。 这些“误报”并不表示该人电子邮件地址的真实有效性。
