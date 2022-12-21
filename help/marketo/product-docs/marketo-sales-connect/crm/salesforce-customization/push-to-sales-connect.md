---
unique-page-id: 14352477
description: 推送至销售连接 — Marketo文档 — 产品文档
title: 推送至Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# 推送至Sales Connect {#push-to-sales-connect}

我们的“推送到输出”按钮将在Salesforce中获取您的潜在客户/联系人列表，并在Sales Connect中将它们推入一个组。 然后，您可以快速发送附加了Tout跟踪的可自定义的组电子邮件。

## 要求 {#requirements}

* 由Salesforce管理员安装的Sales Connect Salesforce包

* 通过Salesforce管理员安装的“推送至销售连接”按钮来列出视图

* 与Sales Connect建立的Salesforce连接，用于用户进行推送

## 操作方法 {#how-to}

1. 单击 **潜在客户/联系人** 选项卡。
1. 切换到“开始”按钮旁边要推送到Sales Connect的列表视图。
1. 单击 **开始**.
1. 选择要推送到输出的所有潜在客户/联系人。
1. 选择 **推送到MSE**.
1. 将显示一个新窗口，用于验证要推送的潜在客户/联系人数量。 选择 **进入组**. Sales Connect不会推送任何在Salesforce中标记为“电子邮件选择退出”或在Sales Connect中标记为“未订阅”的联系人。

   >[!NOTE]
   >
   >Sales Connect将添加标题为“SFDC-..”的组 到 [Web应用程序](https://toutapp.com/login).

1. 选择 **电子邮件整个组** 发送此群组电子邮件。
