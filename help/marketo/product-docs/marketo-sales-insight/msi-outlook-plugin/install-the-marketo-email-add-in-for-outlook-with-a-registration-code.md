---
unique-page-id: 2949711
description: 使用注册代码安装适用于Outlook的Marketo电子邮件加载项 — Marketo文档 — 产品文档
title: 使用注册代码安装适用于Outlook的Marketo Email Add-in
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 268a7f1ca441661e1d943a8d6abce7bdcf308a98
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 使用注册代码安装适用于Outlook的Marketo Email Add-in {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

如果用户可以在其笔记本电脑上访问管理员设置，您可以直接向他们发送注册代码。

如果您尚未收到邀请电子邮件，请联系Marketo管理员以邀请您。

>[!PREREQUISITES]
>
>你必须 [颁发了Marketo Email Add-in许可证](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>在Windows用户文件夹包含非英语字符的PC上不支持安装。 此文件夹由Windows在 `<System Root>\Users\` 根据Windows用户名，如果Windows用户名是非英文名称，则可能包含非英文字符。 请与您的IT团队合作，以验证您是否遇到安装问题。

>[!NOTE]
>
>10/1/20上，最新版本的Outlook插件停止支持离线模式。

## 下载安装程序 {#download-installer}

1. 识别您的 [Microsoft Outlook版本](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)

1. 单击该链接可下载适用于您的Microsoft Outlook版本的安装程序。

   >[!NOTE]
   >
   >目前，以下链接仅在Microsoft Edge中运行，或在Chrome中右键单击鼠标。 对不起。

   | Outlook版本 | 32位Outlook | 64位Outlook |
   |---|---|---|
   | 2000年展望 | 不受支持 | 不适用 |
   | 2003年展望 | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | 不适用 |
   | 2007年展望 | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | 不适用 |
   | 2010年展望 | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下载](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | 2013年展望 | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下载](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | 《2016年展望》 | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下载](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | 《2019年展望》 | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下载](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Mac展望 | 不受支持 | 不受支持 |
   | Outlook Web应用程序 | 不受支持 | 不受支持 |
   | Office 365* | [下载](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [下载](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Office 365版本：仅限Windows客户端（在Windows 10、Enterprise或Pro上）。

## 复制您的注册代码 {#copy-your-registration-code}

1. 复制您收到的邀请电子邮件中的注册代码。

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. 关闭Microsoft Outlook。

   ![](assets/ent-key-close-outlook-hand.png)

## 安装 {#install}

1. 运行安装程序。

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >如果收到安全警告，别担心！ 只需单击 **运行**.

1. 单击 **下一个**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. 填写 **名字**, **姓氏**, **电子邮件地址**，然后复制并粘贴 **注册代码** 从电子邮件转到表单，然后单击 **下一个**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >如果安装失败，请咨询您的IT部门，以确保HTTPS流量不会被阻止。 安装程序需要打开HTTPS流量。

1. 单击 **下一个** 以在默认位置安装。

   ![](assets/select-installation-folder-hand.png)

1. 单击 **下一个**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >如果收到有关未知发布者的安全提示，请单击 **是**.

1. 安装现已完成，请单击 **关闭**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. 现在打开Microsoft Outlook并查看Marketo按钮。

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   太棒了！ 现在Marketo按钮的位置更好了。

了解有关使用Marketo消息和日志与Marketo操作的更多信息。

>[!MORELIKETHIS]
>
>* [使用适用于Outlook的Marketo Email Add-in发送和跟踪电子邮件](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [使用Marketo模板从Outlook发送和跟踪](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

