---
unique-page-id: 11382829
description: IT人员卸载Marketo Outlook插件 — Marketo Docs — 产品文档
title: IT人员卸载Marketo Outlook插件
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# IT {#marketo-outlook-plugin-uninstall-by-it}卸载Marketo Outlook插件

下面介绍IT人员如何远程卸载Marketo Outlook插件。

以“系统”或具有要卸载的/x开关的管理用户帐户的形式运行以下命令行。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

有关疑难解答，您可以启用日志记录以创建输出日志文件。

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

要指定日志文件的位置，可以在命令行中指定文件路径。

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>远程卸载该插件将强制关闭用户计算机上的Outlook。

如果您希望尝试不同的日志记录级别或用户界面级别，请参阅[ Microsoft对交换机](https://support.microsoft.com/en-us/kb/227091)的完整列表。
