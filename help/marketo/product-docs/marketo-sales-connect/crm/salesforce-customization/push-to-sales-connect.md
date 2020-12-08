---
unique-page-id: 14352477
description: 推送至销售连接- Marketo Docs —— 产品文档
title: 推送至销售连接
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# 推送至销售连接 {#push-to-sales-connect}

我们的“推送到输出”按钮将列表Salesforce中的潜在客户／联系人，并将其推入Sales Connect中的组。 然后，您可以快速发送可自定义的组电子邮件，并附加“输出”跟踪。

## 要求 {#requirements}

* Sales Connect [Salesforce包](http://docs.marketo.com/x/C4PS) ，安装者 `Salesforce Admin`

* `Push to Sales Connect`按钮安装到列表视图 `Salesforce Admin`

* 使用Sales Connect建立的Salesforce连接，用于用户进行推送

## 操作方法 {#how-to}

1. 单击Salesforce **中的潜在客户** /联系人选项卡。
1. 切换至您要按下“转到”按钮旁边的“推至销售列表”的视图。
1. 单击“ **开始**”。
1. 选择要推送到输出的所有潜在客户／联系人。
1. 选择 **推送到MSE**。
1. 将出现一个新窗口，验证您要推送的潜在客户／联系人数。 选择 **继续到组**。 Sales Connect在 `will not push over` Salesforce或Sales Connect中 `Email Opt Out` 标记为 `Unsubscribed` 的任何联系人。

   >[!NOTE]
   >
   >Sales Connect将添加标题为“SFDC-...”的此组 到Web应用程序上的“关系 [”页面](http://toutapp.com/login)。

1. 选择“ **通过电子邮件发送** 整个组”以发出此组电子邮件。

