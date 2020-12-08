---
unique-page-id: 1147328
description: 电子邮件中的硬弹回和软弹回- Marketo Docs —— 产品文档
title: 电子邮件中的硬边界和软边界
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# 电子邮件中的硬边界和软边界 {#hard-and-soft-bounces-in-email}

当邮件服务器告知Market该人的电子邮件无法送达时，硬弹回会导致该人的电子邮件地址无效。 软弹跳意味着将电子邮件发送给人时出现问题；这会自动得到解决，有时可能需要数天时间。 硬边界和软边界都由多个 [类别组成](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838)。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 跳出分类 {#bounce-classification}

Marketo中有5个与问题电子邮件投放相关的人字符串。

1. **电子邮件已暂停** -当发生某种类型的硬弹回时，将其设置为“True”。
1. **电子邮件挂起** -原因可能有很多。 这个字段试图解释原因。
1. **电子邮件挂起于**-出现违规弹回时，Marketo将暂停邮寄给该人24小时。
1. **电子邮件无效** -当发生某种类型的硬弹回时，设置为“True”。
1. **电子邮件无效** -硬弹出的原因。

>[!NOTE]
>
>当人员达到电子邮 **件挂起状** 态后，将无法清除电子邮件挂起复选框。 不过，在最初停职24小时后，该人仍可邮寄。
>
>当某人被标记为电子邮 **件无效**，则只能通过取消选中其记录的“人员信息”选项卡中的“电子邮件无效”框来手动重置他们（我们建议您仅在您知道其电子邮件有效时重置）。

>[!NOTE]
>
>**先决条件**
>
>按照 [以下步骤](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) ，创建将生成弹回数据的电子邮件性能报告。

创建电子邮件性能报告后，屏幕应当如下： ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>垃圾邮件过滤器有时会产生硬弹回。 这些“误报”并不表示该人电子邮件地址的真实有效性。

