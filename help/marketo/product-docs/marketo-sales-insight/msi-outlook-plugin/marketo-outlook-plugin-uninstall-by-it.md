---
unique-page-id: 11382829
description: Marketo Outlook插件由IT卸载 — Marketo文档 — 产品文档
title: Marketo Outlook插件由IT卸载
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# Marketo Outlook插件由IT卸载 {#marketo-outlook-plugin-uninstall-by-it}

以下是IT如何远程卸载Marketo Outlook插件。

以“System”形式运行以下命令行，或者运行带有/x开关的管理用户帐户来卸载。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

对于疑难解答，您可以启用日志记录来创建输出日志文件。

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
>远程卸载插件将强制关闭用户计算机上的Outlook。

请参考 [Microsoft的交换机完整列表](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 如果您希望尝试不同的日志记录级别或用户界面级别。
