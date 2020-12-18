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


# 推送到Sales Connect {#push-to-sales-connect}

我们的“推送到输出”按钮将列表Salesforce中的潜在客户／联系人，并将其推入Sales Connect中的组。 然后，您可以快速发送可自定义的组电子邮件，并附加“输出”跟踪。

## 要求{#requirements}

* 由`Salesforce Admin`安装的Sales Connect [Salesforce包](http://docs.marketo.com/x/C4PS)

* `Push to Sales Connect`按钮安装到列表视图  `Salesforce Admin`

* 使用Sales Connect建立的Salesforce连接，用于用户进行推送

## 操作方法{#how-to}

1. 单击Salesforce中的&#x200B;**潜在客户／联系人**&#x200B;选项卡。
1. 切换至您要按下“转到”按钮旁边的“推至销售列表”的视图。
1. 单击&#x200B;**转至**。
1. 选择要推送到输出的所有潜在客户／联系人。
1. 选择&#x200B;**推送到MSE**。
1. 将出现一个新窗口，验证您要推送的潜在客户／联系人数。 选择&#x200B;**继续到组**。 Sales Connect `will not push over`在Salesforce中标为`Email Opt Out`或在Sales Connect中标为`Unsubscribed`的任何联系人。

   >[!NOTE]
   >
   >Sales Connect将添加标题为“SFDC-...”的此组 到[web应用程序](http://toutapp.com/login)上的“关系”页。

1. 选择&#x200B;**电子邮件整个组**&#x200B;以发出此组电子邮件。

