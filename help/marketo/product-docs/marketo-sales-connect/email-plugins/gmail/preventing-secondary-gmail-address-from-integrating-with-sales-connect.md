---
unique-page-id: 14352546
description: 阻止辅助Gmail地址与Sales Connect - Marketo Docs —— 产品文档集成
title: 阻止辅助Gmail地址与Sales Connect集成
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# 阻止辅助Gmail地址与Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}集成

## Gmail集成中断（为什么我的个人Gmail发送电子邮件）{#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Gmail连接中断的最常见原因是与用户个人帐户的意外集成。 当用户单击“Connect”或尝试从其个人帐户发送电子邮件时，会发生这种情况。 这样做可能很诱人，因为当在Chrome的同一实例中访问您的Gmail帐户时，该选项会与您的工作电子邮件相同。

## 为什么Sales Connect甚至尝试与我的个人Gmail集成？{#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect通过Chrome浏览器中安装的扩展与Gmail集成。 只要Gmail的扩展感到Gmail的实例打开，它就会优惠一个与它集成的选项。 为防止与您的个人Gmail帐户集成，我们建议您做以下三件事之一……

以其他Chrome用户身份登录（推荐）

单击[此链接](https://support.google.com/chrome/answer/2364824?hl=en)以了解如何创建其他Chrome用户档案。

**优势**:以其他用户身份登录将打开Chrome的新实例。此实例是Chrome的一个全新窗口，此窗口中不存在任何旧扩展。 它还保存了cookie，因此您不必每次都登录Gmail。

**缺点**:必须打开Chrome的两个窗口。

使用其他浏览器

**专业人** 员：使用未安装扩展的其他因特网浏览器（IE或Firefox）将阻止这种情况发生。

**缺点**:使用多个浏览器可能会很烦人。

使用隐姓埋名窗口

**专业人** 士：隐姓埋名的窗口就像打开Chrome的裸体版本。这意味着它不会安装您的任何扩展，并且Sales Connect也不会在那里连接。

**缺点**:每次开始时，您必须登录到Gmail，如果不小心关闭了窗口，则必须再次登录。
