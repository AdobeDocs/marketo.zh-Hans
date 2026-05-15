---
unique-page-id: 14352540
description: 了解如何防止在Sales Connect中查看自述。 在预览或测试电子邮件时，避免计算您自己的打开次数。
title: 防止自我查看
exl-id: c18715fc-4ca2-4a6b-8f63-a9406f30c0d8
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/UF-7Po7qajqMUjhP0LXWSxDqgqQyauDMLqDACzyWHVc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 2%

---

# 防止自我查看 {#preventing-self-views}

## 概述 {#overview}

获取视图跟踪的误报可能会导致报表不一致。 当MSC的用户意外从其电子邮件客户端调用跟踪像素时，经常会发生这种情况（我们称之为自查看）。 下面是有关大幅减少甚至消除自我看法的一些提示。

## Web （[!DNL Outlook Web App]和Gmail） {#web-outlook-web-app-and-gmail}

[!DNL Sales Connect]将在浏览器中存储Cookie，以防止在从Outlook Web App和Gmail打开电子邮件时跟踪查看次数。 如果您仍在接收自检信息，我们建议您执行以下操作：

* 确保您的计算机上启用了Cookie。

* 如果您使用的是新计算机或移动设备，请确保您已登录Web应用程序。 这将允许我们以后识别您的计算机/设备。

## 桌面(Windows) {#desktop-windows}

通过在电子邮件客户端中下载一个不可见的小图像像素来跟踪视图。 通过禁用自动下载的图像，可以显着降低[!DNL Outlook]中的自检次数。 以下是操作步骤。

1. 在[!DNL Outlook]中，单击菜单栏中的&#x200B;**[!UICONTROL File]**。

   ![](assets/win-1.png)

1. 单击 **[!UICONTROL Options]**。

   ![](assets/win-2.png)

1. 在[!DNL Outlook]选项对话框中，单击&#x200B;**[!UICONTROL Trust Center]**。

   ![](assets/win-3.png)

1. 在[!UICONTROL Microsoft Outlook Trust Center]下，单击&#x200B;**[!UICONTROL Trust Center Settings]**。

   ![](assets/win-4.png)

1. 单击左侧菜单中的[!UICONTROL Automatic Download]，然后选中&#x200B;**[!UICONTROL Don't download pictures automatically in HTML email or RSS items]**&#x200B;复选框。

   ![](assets/win-5.png)

1. 在[!UICONTROL Trust Center]对话框中单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/win-6.png)

1. 在[!DNL Outlook]选项对话框中单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/win-6.png)

## 桌面(Mac) {#desktop-mac}

通过在电子邮件客户端中下载一个不可见的小图像像素来跟踪视图。 通过禁用自动下载的图像，可以显着降低[!DNL Outlook]中的自检次数。 以下是操作步骤。

1. 在[!DNL Outlook]中，单击菜单栏中的&#x200B;**[!UICONTROL Outlook]**&#x200B;并选择&#x200B;**[!UICONTROL Preferences]**。

   ![](assets/mac-1.png)

1. 在[!UICONTROL Email]下，选择&#x200B;**[!UICONTROL Reading]**。

   ![](assets/mac-2.png)

1. 在[!UICONTROL Security]下，单击&#x200B;**[!UICONTROL Never]**&#x200B;单选按钮。

   ![](assets/mac-3.png)
