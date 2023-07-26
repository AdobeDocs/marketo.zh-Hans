---
unique-page-id: 2359504
description: 使用“发件人地址”A/B测试 — Marketo文档 — 产品文档
title: 使用“发件人地址”A/B测试
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 使用“发件人地址”A/B测试 {#use-from-address-a-b-testing}

您可以轻松对电子邮件进行A/B测试。 一个有趣的测试是 **发件人地址** 测试。 下面是设置方法。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在 **电子邮件** 图块，选择电子邮件后，单击 **添加A/B测试**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. 随即会打开一个新窗口，选择 **发件人地址** 对象 **测试类型**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. 如果您具有以前的测试信息（如主题测试），则可以安全地单击 **重置测试**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. 输入第二个 **发件人地址** 要测试的信息。

   >[!NOTE]
   >
   >选项A将预填充选定电子邮件中包含的信息。

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >您可以单击 **+** 以添加所需数量的发件人地址。

1. 使用滑块选择要在A/B测试中显示的受众百分比，然后单击 **下一个**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >不同的变体将发送到所选测试样本大小的相同部分。

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**. 如果您使用静态列表，如果将样本大小设置为100%，则会向受众中的每个人发送电子邮件，并且入选者不会向任何人发送电子邮件。 如果您使用 **智能** 列表，将样本大小设置为100%会向受众中的每个人发送电子邮件 _当时_. 稍后当电子邮件程序再次运行时，任何符合智能列表条件的新用户也将收到电子邮件，因为他们现在包含在受众中。

   好了，我们快到了。 现在我们需要 [定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
