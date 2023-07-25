---
unique-page-id: 2951056
description: 发行说明 — 2013年9月 — Marketo文档 — 产品文档
title: 发行说明 — 2013年9月
exl-id: 43428813-0405-4c35-9165-f189fbb5ffb7
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 发行说明： 2013年9月 {#release-notes-september}

9月版本中包含以下功能。

## 较短的URL {#shorter-urls}

已修剪电子邮件URL，使其对收件人单击友好，同时保留所有跟踪功能

>[!CAUTION]
>
>当我们切换到“短URL”时，在9月版本之前发送的电子邮件中的链接将在本版本发布90天后过期。

使用Marketo自定义对象中的数据，或使用Velocity模板语言向电子邮件内容添加条件逻辑。

![](assets/image2014-9-22-17-3a10-3a56.png)

## 更改发送测试以发送示例 {#change-send-test-to-send-sample}

我们已将发送测试重命名为发送示例

## 个性化发送示例电子邮件 {#personalized-send-sample-email}

在发送电子邮件示例时，您可以选择潜在客户的名称以个性化示例电子邮件。

![](assets/image2014-9-22-17-3a11-3a22.png)

## goToWebinar的其他字段同步 {#additional-field-sync-for-gotowebinar}

您可以将Marketo表单中的公司名称和职称同步到GoTo网络研讨会。 要启用这些附加字段，请转到Event Partners并选中“Enable Additional Fields”。

![](assets/image2014-9-22-17-3a11-3a53.png)

## 限制用户仅登录SSO {#restrict-user-login-to-sso-only}

将订阅配置为仅允许Marketo用户通过SSO登录，而不通过普通登录屏幕登录

## 已上传文件的病毒扫描 {#virus-scan-of-uploaded-files}

现在，如果上传到Design Studio的文件包含病毒，则会自动扫描并阻止这些文件

## 导出机会影响分析器 {#export-opportunity-influence-analyzer}

您现在可以将Opportunity Influence Analyzer中的数据导出到Excel。 每个导出的Excel文件都包含所有潜在客户（包括在商机中没有角色的潜在客户）的所有营销交互，以及分析器中选定帐户下的所有商机。 机会行以绿色突出显示。 如果您需要专注于特定的潜在客户或营销活动，则可以使用Excel的本机数据筛选功能。

![](assets/image2014-9-22-17-3a12-3a23.png)

## 项目归因设置 {#program-attribution-settings}

您可以更改Marketo在首次接触和多次接触归因量度中关联联系人和商机的方式，包括执行基于帐户的归因的功能。 这些设置将影响Program Opportunity Analysis区域和Opportunity Analysis区域下的Revenue Explorer报表中的归因指标。 这也将影响Program Analyzer中的归因指标。

您可以将项目归因设置更改为三个选项之一。 更改此设置不会修改任何Marketo或CRM数据；它只会更改报表的运行方式，并且可随时还原。

Explicit设置将只检查具有角色的联系人（当前行为）。 隐式将检查与帐户关联的所有联系人，而不管角色如何。 我们强烈建议尽可能使用显式模式。 使用“隐含”可能会产生误报，即认为机会有价值的人尽管对机会没有真正的影响力。

![](assets/image2014-9-22-17-3a12-3a43.png)

## Sales Insight提供法语版和德语版（仅限Salesforce） {#sales-insight-available-in-french-and-german-salesforce-only}

从AppExchange下载最新版本的Marketo Lead Management和Marketo Sales Insight ，以便您的法语和德语销售人员能够以他们的首选语言查看Sales Insight内容。

![](assets/image2014-9-22-17-3a13-3a12.png)

## Cobalt用户界面 {#cobalt-user-interface}

在接下来的几个月中，将在应用程序的不同部分推出新的主题。 本月，您可能会注意到更多新的蓝色模式窗口。
