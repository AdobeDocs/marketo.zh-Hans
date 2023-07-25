---
unique-page-id: 14352540
description: 阻止自行查看 — Marketo文档 — 产品文档
title: 阻止自我查看
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 阻止自我查看 {#preventing-self-views}

## 概述 {#overview}

获取视图跟踪的误报可能会导致报表不一致。 当MSC用户意外从其电子邮件客户端调用跟踪像素时，经常会发生这种情况（我们称之为自查看）。 下面是一些关于显着减少甚至消除自我视图的提示。

## Web（Outlook Web App和Gmail） {#web-outlook-web-app-and-gmail}

Sales Connect将在您的浏览器中存储Cookie，以防止在从Outlook Web App和Gmail打开电子邮件时跟踪查看次数。 如果您仍在接收自检信息，我们建议您执行以下操作：

* 确保您的计算机上启用了Cookie。

* 如果您使用的是新计算机或移动设备，请确保您已登录Web应用程序。 这将允许我们识别您的计算机/设备。

## 桌面(Windows) {#desktop-windows}

通过在电子邮件客户端中下载一个不可见的小图像像素来跟踪视图。 通过禁用自动下载的图像，可以显着降低Outlook中自我查看的次数。 以下是操作步骤。

1. 在Outlook中，单击 **文件** 在菜单栏中。

   ![](assets/win-1.png)

1. 单击 **选项**.

   ![](assets/win-2.png)

1. 在“Outlook选项”对话框中，单击 **托管中心**.

   ![](assets/win-3.png)

1. 在Microsoft Outlook信任中心下，单击 **信任中心设置**.

   ![](assets/win-4.png)

1. 单击左侧菜单中的“自动下载”，然后选择 **不要自动下载HTML电子邮件或RSS项目中的图片** 复选框。

   ![](assets/win-5.png)

1. 单击 **确定** 在“信任中心”对话框中。

   ![](assets/win-6.png)

1. 单击 **确定** 在Outlook选项对话框中。

   ![](assets/win-6.png)

## 桌面(Mac) {#desktop-mac}

通过在电子邮件客户端中下载一个不可见的小图像像素来跟踪视图。 通过禁用自动下载的图像，可以显着降低Outlook中自我查看的次数。 以下是操作步骤。

1. 在Outlook中，单击 **Outlook** 在菜单栏中选择 **首选项**.

   ![](assets/mac-1.png)

1. 在电子邮件下，选择 **阅读**.

   ![](assets/mac-2.png)

1. 在Security下，单击 **从不** 单选按钮。

   ![](assets/mac-3.png)
