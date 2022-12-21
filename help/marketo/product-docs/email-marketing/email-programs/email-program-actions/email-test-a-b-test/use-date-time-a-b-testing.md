---
unique-page-id: 2359520
description: 使用“日期/时间”A/B测试 — Marketo文档 — 产品文档
title: 使用“日期/时间”A/B测试
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 使用“日期/时间”A/B测试 {#use-date-time-a-b-testing}

您可以轻松地A/B测试电子邮件。 一个测试是 **日期/时间** 测试。 此测试最适合在一天中或一天中的哪个时间发送电子邮件。 下面是如何设置它。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在 **电子邮件** 拼贴，单击 **添加A/B测试**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. 将打开一个新窗口。 选择 **日期/时间** 表示 **测试类型**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. 如果您之前有测试信息（如主题测试），则可以安全地单击 **重置测试**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. 选择首个日期/时间的日期。

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. 选择您的首次日期/时间的时间。

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. 对第二个日期/时间执行相同操作。

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. 使用滑块选择A/B测试中所需受众的百分比，然后单击 **下一个**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >不同的变体将应用于所选测试样本量的相等部分。

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**. 如果您使用的是静态列表，则将示例大小设置为100%会向受众中的每个人发送电子邮件，而入选者将不会发送给任何人。 如果您使用 **智能** 列表时，将示例大小设置为100%会向受众中的每个人发送电子邮件 _那时_. 当电子邮件程序在以后的日期再次运行时，任何符合智能列表资格的新用户也将收到电子邮件，因为他们现在已包含在受众中。

   好，我们离这一步更近了。 现在我们需要 [定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
