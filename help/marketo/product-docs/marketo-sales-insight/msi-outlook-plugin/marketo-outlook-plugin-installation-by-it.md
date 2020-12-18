---
unique-page-id: 11382815
description: IT的Marketo Outlook插件安装- Marketo Docs —— 产品文档
title: IT人员安装Marketo Outlook插件
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# IT {#marketo-outlook-plugin-installation-by-it}安装Marketo Outlook插件

有时，公司策略要求其IT团队在其员工的计算机上安装所有软件。 在这些情况下，IT经常使用自己的部署软件远程完成此操作。 本文档提供了在部署过程中用作输入以远程安装Outlook插件的命令行。

>[!PREREQUISITES]
>
>[设置](http://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) 企业密钥。

以“系统”或“管理”用户帐户的形式运行以下命令行，并使用/i开关进行安装。 `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

对于疑难解答，您可以启用日志记录以创建输出日志文件。 `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

要指定日志文件的位置，可以在命令行中指定文件路径。 `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>日志文件的存储位置必须存在，否则安装将中止。

如果要尝试不同的日志记录级别或用户界面级别，请参阅[Microsoft的交换机完整列表](https://support.microsoft.com/en-us/kb/227091)。

>[!NOTE]
>
>**相关文章**
>
>[IT人员卸载Marketo Outlook插件](marketo-outlook-plugin-uninstall-by-it.md)

