---
unique-page-id: 14352546
description: 阻止将次要Gmail地址与Sales Connect集成 — Marketo文档 — 产品文档
title: 防止辅助 Gmail 地址与 Sales Connect 集成
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# 阻止次要Gmail地址与[!DNL Sales Connect]集成 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail集成损坏（为什么我的个人Gmail会发送电子邮件） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail连接中断的最常见原因是与用户的个人帐户意外集成。 当用户单击“连接”或尝试从其个人帐户发送电子邮件时，可能会发生这种情况。 这可能非常诱人，因为在与工作电子邮件相同的[!DNL Chrome]实例中访问您的Gmail帐户时，将存在该选项。

## 为什么[!DNL Sales Connect]甚至尝试与我的个人Gmail集成？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect]通过[!DNL Chrome]浏览器中安装的扩展与Gmail集成。 每当扩展检测到Gmail的实例打开时，它都会提供一个选项来与它集成。 为了防止与您的个人Gmail帐户集成，我们建议您执行以下三件事之一……

以其他[!DNL Chrome]用户登录（推荐）

单击[此链接](https://support.google.com/chrome/answer/2364824?hl=en)了解如何创建另一个[!DNL Chrome]配置文件。

**属性**：以其他用户身份登录将打开[!DNL Chrome]的新实例。 此实例是[!DNL Chrome]的全新窗口，此窗口中不会存在任何旧扩展。 它还保留Cookie，因此您不必每次都登录Gmail。

**缺点**：必须打开两个[!DNL Chrome]窗口。

使用其他浏览器

**优点：**&#x200B;使用另一个未安装扩展的Internet浏览器（IE或Firefox）将阻止发生这种情况。

**缺点**：使用多个浏览器可能令人讨厌。

使用无痕窗口

**优点：**&#x200B;无痕窗口就像打开裸体版本的[!DNL Chrome]。 这意味着它不会安装您的任何扩展，并且[!DNL Sales Connect]将不在那里进行连接。

**问题**：每次开始工作时，都必须登录Gmail，如果意外关闭窗口，则必须再次登录。
