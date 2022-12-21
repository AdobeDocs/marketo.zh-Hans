---
unique-page-id: 2359504
description: 使用“发件人地址”A/B测试 — Marketo文档 — 产品文档
title: 使用“发件人地址”A/B测试
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 使用“发件人地址”A/B测试 {#use-from-address-a-b-testing}

您可以轻松地A/B测试电子邮件。 一个有趣的测试是 **发件人地址** 测试。 下面是如何设置它。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在 **电子邮件** 拼贴，在选择您的电子邮件后，单击 **添加A/B测试**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. 打开新窗口，选择 **发件人地址** 表示 **测试类型**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. 如果您之前有测试信息（如主题测试），则可以安全地单击 **重置测试**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. 输入第二个 **发件人地址** 要测试的信息。

   >[!NOTE]
   >
   >选择A将预填充选定电子邮件中包含的信息。

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >您可以单击 **+** 添加任意所需数量的发件人地址。

1. 使用滑块选择A/B测试中所需受众的百分比，然后单击 **下一个**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >不同的变体将发送到所选测试样本大小的相等部分。

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**. 如果您使用的是静态列表，则将示例大小设置为100%会向受众中的每个人发送电子邮件，而入选者将不会发送给任何人。 如果您使用 **智能** 列表时，将示例大小设置为100%会向受众中的每个人发送电子邮件 _那时_. 当电子邮件程序在以后的日期再次运行时，任何符合智能列表资格的新用户也将收到电子邮件，因为他们现在已包含在受众中。

   好，我们快到了。 现在我们需要 [定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
