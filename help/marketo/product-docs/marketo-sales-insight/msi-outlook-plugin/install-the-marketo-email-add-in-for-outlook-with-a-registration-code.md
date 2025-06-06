---
unique-page-id: 2949711
description: 安装适用于Outlook的Marketo电子邮件加载项，并提供注册码 — Marketo文档 — 产品文档
title: 使用注册码安装适用于Outlook的Marketo电子邮件加载项
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: ac6c84a82b9bcb535d5f50897d1a068a5a746287
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 3%

---

# 使用注册码安装适用于Outlook的Marketo电子邮件加载项 {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

如果用户能够访问其笔记本电脑上的管理员设置，则可以直接向他们发送注册码。

如果您没有收到邀请电子邮件，请咨询Marketo管理员以邀请您。

>[!PREREQUISITES]
>
>您必须是[颁发的Marketo电子邮件加载项许可证](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md)。

>[!IMPORTANT]
>
>在Windows用户文件夹包含非英语字符的PC上不支持安装。 此文件夹由Windows在`<System Root>\Users\`下基于Windows用户名自动生成，如果Windows用户名是非英文名称，则可能包含非英文字符。 请与您的IT团队合作，验证您是否遇到安装问题。

>[!NOTE]
>
>Sales Insight Actions功能（包括“发送销售电子邮件”、“添加到Sales Campaign”和“任务”）在Gmail和Outlook的Sales Insight电子邮件插件中不可用。 目前，在使用Sales Insight电子邮件插件时，用户只能从其电子邮件客户端发送可跟踪电子邮件，无论是否包含Marketo电子邮件模板。

## 下载安装程序 {#download-installer}

1. 识别您的[Microsoft Outlook版本](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}。

1. 在下表中，单击链接以下载适用于您的Microsoft Outlook版本的.ZIP文件。

1. 解压缩文件以访问所需的.MSI文件，然后继续安装。

   >[!NOTE]
   >
   >目前，以下链接仅在Microsoft Edge中有效，或者通过在Chrome中右键单击有效。 造成任何不便，敬请见谅。

<table><thead>
  <tr>
    <th>Outlook版本</th>
    <th>32位Outlook</th>
    <th>64位Outlook</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>不支持</td>
    <td>不适用</td>
  </tr>
  <tr>
    <td>2003年展望</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td>不适用</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td>不适用</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下载</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下载</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下载</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下载</a></td>
  </tr>
  <tr>
    <td>适用于Mac的Outlook</td>
    <td>不支持</td>
    <td>不支持</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>不支持</td>
    <td>不支持</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">下载</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">下载</a></td>
  </tr>
</tbody></table>

*Office 365版本：仅限Windows客户端（在Windows 10、Enterprise或Pro上）。

>[!IMPORTANT]
>
>Microsoft已发布适用于Windows[&#128279;](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}的新版Outlook。 此新版本不支持现有的MSI Outlook插件。 MSI Outlook插件将继续用于运行经典版本的Outlook的Windows桌面。 若要了解有关适用于组织的新Outlook for Windows的详细信息，请[单击此处](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}。

## 复制您的注册码 {#copy-your-registration-code}

1. 从您收到的邀请电子邮件中复制注册码。

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. 关闭Microsoft Outlook。

   ![](assets/ent-key-close-outlook-hand.png)

## 安装 {#install}

1. 运行安装程序。

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >如果您收到安全警告，请不要担心！ 只需单击&#x200B;**运行**。

1. 单击&#x200B;**下一步**。

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. 填写&#x200B;**名字**、**姓氏**、**电子邮件地址**，然后将电子邮件中的&#x200B;**注册码**&#x200B;复制并粘贴到表单中，然后单击&#x200B;**下一步**。

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >如果安装失败，请与IT部门联系，以确保不会阻止HTTPS流量。 安装程序要求打开HTTPS流量。

1. 单击&#x200B;**下一步**&#x200B;安装在默认位置。

   ![](assets/select-installation-folder-hand.png)

1. 单击&#x200B;**下一步**。

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >如果收到有关未知发布者的安全提示，请单击&#x200B;**是**。

1. 安装现已完成，请单击&#x200B;**关闭**。

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. 现在打开Microsoft Outlook并查看Marketo按钮。

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   太棒了！ 现在，Marketo按钮占据了一个更好的位置。

了解有关使用Marketo消息和日志与Marketo操作的更多信息。

>[!MORELIKETHIS]
>
>* [使用适用于Outlook的Marketo电子邮件加载项发送和跟踪电子邮件](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [使用Marketo模板从Outlook发送和跟踪](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
