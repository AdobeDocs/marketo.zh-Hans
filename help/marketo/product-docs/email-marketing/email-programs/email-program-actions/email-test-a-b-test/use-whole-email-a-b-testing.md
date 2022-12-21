---
unique-page-id: 2359502
description: 使用“整个电子邮件”A/B测试 — Marketo文档 — 产品文档
title: 使用“整个电子邮件”A/B测试
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 使用“整个电子邮件”A/B测试 {#use-whole-email-a-b-testing}

您可以轻松地A/B测试电子邮件。 一个很棒的考验是 **整封电子邮件** 测试。 下面是如何设置它。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在电子邮件拼贴下，选择您的电子邮件后，单击 **添加A/B测试**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. 将打开一个新窗口。 单击 **测试类型** 下拉框并选择 **整封电子邮件**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. 如果您之前有测试信息（如主题测试），则可以安全地单击 **重置测试**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. 选择您的第一封电子邮件。

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. 单击 **添加** 以应用电子邮件。

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >您可以添加多封电子邮件。 但是，如果添加的量过多，可能会减慢测试过程。

1. 选择您的第二封电子邮件。

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. 单击 **添加** 以应用第二封电子邮件。 拖动滑块以选择您希望接收A/B测试的受众百分比，然后单击 **下一个**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >不同的变体将发送到所选内容的相同部分 **测试样本量**.

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**. 如果您使用的是静态列表，则将示例大小设置为100%会向受众中的每个人发送电子邮件，而入选者将不会发送给任何人。 如果您使用 **智能** 列表时，将示例大小设置为100%会向受众中的每个人发送电子邮件 _那时_. 当电子邮件程序在以后的日期再次运行时，任何符合智能列表资格的新用户也将收到电子邮件，因为他们现在已包含在受众中。

   好，我们快到了。 现在我们需要 [定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
