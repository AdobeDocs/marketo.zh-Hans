---
unique-page-id: 11382815
description: 由IT人员安装的Marketo Outlook插件 — Marketo文档 — 产品文档
title: 由IT人员安装的Marketo Outlook插件
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# 由IT人员安装的Marketo Outlook插件 {#marketo-outlook-plugin-installation-by-it}

有时，公司政策要求其IT团队在员工计算机上安装所有软件。 在这些情况下， IT通常使用自己的部署软件远程执行这一操作。 本文档提供了在部署过程中用作输入以远程安装Outlook插件的命令行。

>[!PREREQUISITES]
>
>[设置](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) 企业密钥。

以“System”形式运行以下命令行，或者运行带有/i开关的“管理”用户帐户来安装。

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

对于疑难解答，可以启用日志记录以创建输出日志文件。

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

要指定日志文件的位置，可以在命令行中指定文件路径。

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>日志文件的存储位置必须存在，否则安装将中止。

请参阅 [Microsoft的交换机完整列表](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 如果您希望尝试不同的日志记录级别或用户界面级别。

>[!MORELIKETHIS]
>
>[Marketo Outlook插件由IT卸载](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
