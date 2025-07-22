---
unique-page-id: 14746177
description: 重新订阅和取消订阅 — Marketo文档 — 产品文档
title: 重新订阅和取消订阅
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 重新订阅[!UICONTROL Unsubscribe] {#resubscribing-an-unsubscribe}

有时候，人们会希望选择重新接收电子邮件。 下面是如何使取消订阅再次成为可发送邮件的。

>[!NOTE]
>
>**需要管理员权限**

>[!CAUTION]
>
>在重新订阅某个人之前，您应该能够证明已记录重新订阅该人员的授权并遵守所有适用法律。

>[!NOTE]
>
>如果已打开取消订阅同步，则必须从ToutApp中删除取消订阅并取消选中[!DNL Salesforce]中的选择退出，以便人员记录不再同步。

1. 转到[Web应用程序](https://toutapp.com/login)并单击&#x200B;**[!UICONTROL People]**。

1. 选择人员以打开人员详细信息视图。

   ![](assets/two.png)

1. 单击人员详细信息视图中的三个圆点，然后选择&#x200B;**[!UICONTROL Remove Unsubscribe]**。

   ![](assets/three.png)

1. 选择选择人员重新加入接收电子邮件的原因，然后单击&#x200B;**[!UICONTROL Remove Unsubscribe]**。

   ![](assets/four.png)

>[!NOTE]
>
>如果已打开unsubscribe同步，则必须同时在Salesforce中取消选中记录上的选择退出框，否则夜间同步将在[!DNL Sales Connect]中重新取消订阅该人员，因为它将检测到该人员在[!DNL Salesforce]中被选择退出。 如果其中任何一条记录被选择退出/取消订阅，则同步会将链接的记录标记为此类记录。
