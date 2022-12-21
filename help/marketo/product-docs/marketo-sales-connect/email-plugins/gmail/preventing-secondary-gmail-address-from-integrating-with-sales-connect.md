---
unique-page-id: 14352546
description: 阻止次级Gmail地址与Sales Connect集成 — Marketo文档 — 产品文档
title: 阻止次级Gmail地址与Sales Connect集成
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 阻止次级Gmail地址与Sales Connect集成 {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Gmail集成中断（为什么我的个人Gmail发送电子邮件） {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail连接断开的最常见原因是与用户个人帐户的意外集成。 当用户单击“连接”或尝试从其个人帐户发送电子邮件时，可能会发生这种情况。 这样做非常有诱惑力，因为在与工作电子邮件相同的Chrome实例中访问您的Gmail帐户时，将会存在该选项。

## 为什么Sales Connect会尝试与我的个人Gmail集成？ {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect通过Chrome浏览器中安装的扩展与Gmail集成。 每当该扩展感知到Gmail的实例打开时，它都会提供一个与其集成的选项。 为防止与您的个人Gmail帐户集成，我们建议您从以下三个方面选择一种……

以其他Chrome用户身份登录（推荐）

单击 [此链接](https://support.google.com/chrome/answer/2364824?hl=en) 了解如何创建其他Chrome配置文件。

**优点**:以其他用户身份登录将打开Chrome的新实例。 此实例是Chrome的全新窗口，且此窗口中不存在任何旧扩展。 它还会保存Cookie，这样您就不必每次都登录Gmail。

**缺点**:必须打开Chrome的两个窗口。

使用其他浏览器

**优点：** 如果使用其他未安装扩展的Internet浏览器（IE或Firefox），则将阻止发生此情况。

**缺点**:使用多个浏览器可能会很烦人。

使用隐身窗口

**优点：** 隐身窗口就像打开Chrome的裸体版本。 这意味着它将未安装您的任何扩展，并且Sales Connect将不会存在进行连接。

**缺点**:每次开始工作时，您都必须登录Gmail，如果意外关闭了窗口，则必须再次登录。
