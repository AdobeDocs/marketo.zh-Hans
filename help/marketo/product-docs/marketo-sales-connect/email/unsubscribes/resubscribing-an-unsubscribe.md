---
unique-page-id: 14746177
description: 重新订阅取消订阅 — Marketo文档 — 产品文档
title: 重新订阅取消订阅
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# 重新订阅取消订阅 {#resubscribing-an-unsubscribe}

有时，人们会想要选择退回接收电子邮件。 下面介绍如何使取消订阅的邮件再次发送。

>[!NOTE]
>
>**需要管理员权限**

>[!CAUTION]
>
>在重新订阅某人之前，您应该能够证明重新订阅授权已记录并符合所有适用法律。

>[!NOTE]
>
>如果已打开取消订阅同步，则必须从ToutApp中删除取消订阅，并在Salesforce中取消选择退订，以便人员记录不再同步。

1. 转到 [Web应用程序](https://toutapp.com/login) 单击 **人员**.

1. 选择人员以打开人员详细信息视图。

   ![](assets/two.png)

1. 单击“人员详细信息”视图中的三个圆点，然后选择 **删除取消订阅**.

   ![](assets/three.png)

1. 选择人员被选择回访以接收电子邮件的原因，然后单击 **删除取消订阅**.

   ![](assets/four.png)

>[!NOTE]
>
>如果已打开取消订阅同步，则必须在Salesforce中取消选中记录中的选择退订框，否则夜间同步将在Sales Connect中重新取消该人员的订阅，因为它将检测到该人员在Salesforce中已选择退订。 如果其中任一记录被选择退订/取消订阅，则同步将如此标记链接的记录。
