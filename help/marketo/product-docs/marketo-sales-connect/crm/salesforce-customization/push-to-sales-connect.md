---
unique-page-id: 14352477
description: 推送到Sales Connect - Marketo文档 — 产品文档
title: 推送到Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 推送到Sales Connect {#push-to-sales-connect}

我们的“推送到Tout”按钮将获取您在Salesforce中的销售线索/联系人列表，并将他们推送到Sales Connect中的组。 然后，您可以快速发送附加了转出跟踪的可自定义群组电子邮件。

## 要求 {#requirements}

* 由Salesforce管理员安装的Sales Connect Salesforce软件包

* “推送到Sales Connect”按钮已安装，列出由Salesforce管理员显示的视图

* 使用Sales Connect建立的Salesforce Connection供进行推送的用户使用

## 操作方法 {#how-to}

1. 单击 **潜在客户/联系人** 选项卡。
1. 切换到Go按钮旁边要推送到Sales Connect的List View。
1. 单击 **开始**.
1. 选择您要推送至推播的所有潜在客户/联系人。
1. 选择 **推送到MSE**.
1. 将出现一个新窗口，验证您要推移的潜在客户/联系人的数量。 选择 **转到组**. Sales Connect不会推送任何在Salesforce中标记为“电子邮件选择退出”或Sales Connect中标记为“已取消订阅”的联系人。

   >[!NOTE]
   >
   >Sales Connect会将此标题为“SFDC-...”的组添加到 [Web应用程序](https://toutapp.com/login).

1. 选择 **向整个组发送电子邮件** 以发送此群电子邮件。
