---
unique-page-id: 2359494
description: 使用“主题行”A/B测试 — Marketo文档 — 产品文档
title: 使用“主题行”A/B测试
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 使用“主题行”A/B测试 {#use-subject-line-a-b-testing}

您可以轻松地A/B测试电子邮件。 最常见的测试之一是 **主题行** 测试。

>[!PREREQUISITES]
>
>[添加A/B测试](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 在“电子邮件”拼贴下，选择您的电子邮件后，单击添加A/B测试。

![](assets/image2014-9-12-15-3a6-3a2.png)

1. 将打开测试编辑器窗口。 输入一个或多个新主题行。

   >[!NOTE]
   >
   >选择 **A** 将预填充选定电子邮件中包含的信息。

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >您可以单击 **+** 添加更多主题行。

1. 使用滑块选择要接收A/B测试的受众百分比，然后单击 **下一个**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**我们建议您避免将样本大小设置为100%**. 如果您使用的是静态列表，则将示例大小设置为100%会向受众中的每个人发送电子邮件，入选者将不会发送给任何人。 如果您使用智能列表，则将示例大小设置为100%会向受众中的每个人发送电子邮件 _那时_. 当电子邮件程序在以后的日期再次运行时，任何符合智能列表资格的新用户也会收到电子邮件，因为他们现在已包含在受众中。

   >[!NOTE]
   >
   >不同的主题变体将占用所选测试样本量的偶数部分。

   好，我们快到了。 现在我们需要 [定义A/B测试入选者标准](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
