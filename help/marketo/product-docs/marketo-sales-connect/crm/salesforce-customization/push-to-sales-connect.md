---
unique-page-id: 14352477
description: 了解如何使用Salesforce中的“推送到Sales Connect”按钮。 只需单击一下即可将潜在客户或联系人从Salesforce添加到Sales Connect。
title: 推送到 [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/piy3bPtiO48FQhWEmpu5qo4denlJ8v1ZU-VXBlWh0Mg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 166
ht-degree: 1%

---

# 推送到[!DNL Sales Connect] {#push-to-sales-connect}

我们的[!UICONTROL Push to Tout]按钮将获取您在[!DNL Salesforce]中的潜在客户/联系人列表，并将他们推送到[!DNL Sales Connect]中的组。 然后，您可以快速发送附加了转出跟踪的可自定义群组电子邮件。

## 要求 {#requirements}

* 由[!DNL Salesforce]管理员安装的[!DNL Sales Connect Salesforce]包

* 已安装[!UICONTROL Push to Sales Connect]按钮以列出[!DNL Salesforce]管理员的视图

* 与[!DNL Sales Connect]建立的[!DNL Salesforce]连接用于发出推送的用户

## 操作方法 {#how-to}

1. 单击[!DNL Salesforce]中的&#x200B;**[!UICONTROL Lead/Contact]**&#x200B;选项卡。
1. 切换到[!UICONTROL Go]按钮旁边要推送到[!DNL Sales Connect]的列表视图。
1. 单击 **[!UICONTROL Go]**。
1. 选择您要推送至推播的所有潜在客户/联系人。
1. 选择 **[!UICONTROL Push to MSE]**。
1. 将出现一个新窗口，验证您要推移的潜在客户/联系人的数量。 选择&#x200B;**[!UICONTROL Proceed to Group]**.[!DNL Sales Connect] 将不会推送[!DNL Salesforce]中标记为[!UICONTROL Email Opt Out]或[!DNL Sales Connect]中标记为[!UICONTROL Unsubscribed]的任何联系人。

   >[!NOTE]
   >
   >[!DNL Sales Connect]将添加此名为“SFDC-...”的组 到[Web应用程序](https://toutapp.com/login)上的“关系”页面。

1. 选择&#x200B;**[!UICONTROL Email Entire Group]**&#x200B;以发送此群电子邮件。
