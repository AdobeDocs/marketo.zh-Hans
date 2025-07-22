---
unique-page-id: 2359494
description: 使用“主题行”A/B测试 — Marketo文档 — 产品文档
title: 使用“主题行”A/B测试
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 使用“主题行”A/B测试 {#use-subject-line-a-b-testing}

您可以轻松对电子邮件进行A/B测试。 最常见的测试之一是&#x200B;**[!UICONTROL Subject Line]**&#x200B;测试。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在&#x200B;**[!UICONTROL Email tile]**&#x200B;下，选择您的电子邮件后，单击&#x200B;**[!UICONTROL Add A/B Test]**。

![](assets/image2014-9-12-15-3a6-3a2.png)

1. 将会打开测试编辑器窗口。 输入一个或多个新的主题行。

   >[!NOTE]
   >
   >选项&#x200B;**A**&#x200B;将预填充选定电子邮件中包含的信息。

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >您可以单击&#x200B;**+**&#x200B;以添加更多主题行。

1. 使用滑块选择要接收A/B测试的受众百分比，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**。 如果您使用静态列表，如果将样本大小设置为100%，则会向受众中的每个人发送电子邮件，并且入选者不会向任何人发送电子邮件。 如果您使用智能列表，如果将样本大小设置为100%，则会在当时&#x200B;_向受众_&#x200B;中的每个人发送电子邮件。 此外，当电子邮件程序在以后再次运行时，任何符合智能列表条件的新用户都将收到电子邮件，因为他们现在包含在受众中。

   >[!NOTE]
   >
   >不同的主题变体甚至会占用所选测试样本大小的一部分。

   好了，我们快到了。 现在我们需要[定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)。
