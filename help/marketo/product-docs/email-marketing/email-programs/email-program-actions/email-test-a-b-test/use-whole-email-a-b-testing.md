---
unique-page-id: 2359502
description: 使用“整个电子邮件”A/B测试 — Marketo文档 — 产品文档
title: 使用“整个电子邮件”A/B测试
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# 使用“整个电子邮件”A/B测试 {#use-whole-email-a-b-testing}

您可以轻松对电子邮件进行A/B测试。 一个很好的测试是&#x200B;**整个电子邮件**&#x200B;测试。 下面是设置方法。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在“电子邮件”拼贴下，选择您的电子邮件后，单击&#x200B;**[!UICONTROL Add A/B Test]**。

![](assets/image2014-9-12-15-3a22-3a12.png)

1. 此时将打开一个新窗口。 单击&#x200B;**[!UICONTROL Test Type]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Whole Emails]**。

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. 如果您以前有测试信息（如主题测试），则可以安全地单击&#x200B;**[!UICONTROL Reset Test]**。

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. 选择您的第一封电子邮件。

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;以应用电子邮件。

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >您可以添加多个电子邮件。 但是，如果添加太多，可能会降低测试过程的速度。

1. 选择您的第二封电子邮件。

   [&#128279;](assets/image2014-9-12-15-3a23-3a49.png)

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;以应用第二封电子邮件。 拖动滑块以选择要接收A/B测试的受众百分比，然后单击&#x200B;**[!UICONTROL Next]**。

   [&#128279;](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >不同的变体将发送到所选的&#x200B;**测试样本大小**&#x200B;的相同部分。

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**。 如果您使用静态列表，如果将样本大小设置为100%，则会向受众中的每个人发送电子邮件，并且入选者不会向任何人发送电子邮件。 如果您使用的是&#x200B;**智能**&#x200B;列表，如果将样本大小设置为100%，则会在&#x200B;_时向受众_&#x200B;中的每个人发送电子邮件。 稍后当电子邮件程序再次运行时，任何符合智能列表条件的新用户也将收到电子邮件，因为他们现在包含在受众中。

   好了，我们快到了。 现在我们需要[定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)。
