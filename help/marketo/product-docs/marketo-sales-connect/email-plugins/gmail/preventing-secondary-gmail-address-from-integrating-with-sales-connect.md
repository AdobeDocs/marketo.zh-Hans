---
unique-page-id: 14352546
description: 阻止将次要Gmail地址与Sales Connect集成 — Marketo文档 — 产品文档
title: 阻止次要Gmail地址与Sales Connect集成
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 阻止次要Gmail地址与Sales Connect集成 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail集成损坏（为什么我的个人Gmail会发送电子邮件） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail连接中断的最常见原因是与用户的个人帐户意外集成。 当用户单击“连接”或尝试从其个人帐户发送电子邮件时，可能会发生这种情况。 这可能很有吸引力，因为在与工作电子邮件相同的Chrome实例中访问Gmail帐户时，该选项将存在。

## 为什么Sales Connect甚至尝试与我的个人Gmail集成？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect通过安装在Chrome浏览器中的扩展与Gmail集成。 每当扩展检测到Gmail的实例打开时，它都会提供一个选项来与它集成。 为了防止与您的个人Gmail帐户集成，我们建议您执行以下三件事之一……

以其他Chrome用户身份登录（推荐）

单击 [此链接](https://support.google.com/chrome/answer/2364824?hl=en) 以了解如何创建另一个Chrome配置文件。

**优点**：以其他用户身份登录将打开新的Chrome实例。 此实例是全新的Chrome窗口，并且此窗口中将不存在任何旧扩展。 它还保留Cookie，因此您不必每次都登录Gmail。

**缺点**：必须打开两个Chrome窗口。

使用其他浏览器

**优点：** 使用另一个未安装扩展的Internet浏览器（IE或Firefox）会阻止这种情况发生。

**缺点**：使用多个浏览器可能令人讨厌。

使用无痕窗口

**优点：** 无痕窗口就像打开Chrome的裸体版本。 这意味着，它不会安装您的任何扩展，并且Sales Connect将不在那里进行连接。

**缺点**：每次开始工作时，都必须登录到Gmail，如果意外关闭窗口，必须再次登录。
