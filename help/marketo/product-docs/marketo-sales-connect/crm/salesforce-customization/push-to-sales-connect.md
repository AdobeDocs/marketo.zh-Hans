---
unique-page-id: 14352477
description: 推送到 [!DNL Sales Connect] - Marketo文档 — 产品文档
title: 推送到 [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 2%

---

# 推送到[!DNL Sales Connect] {#push-to-sales-connect}

我们的[!UICONTROL Push to Tout]按钮将获取您在[!DNL Salesforce]中的潜在客户/联系人列表，并将他们推送到[!DNL Sales Connect]中的组。 然后，您可以快速发送附加了转出跟踪的可自定义群组电子邮件。

## 要求 {#requirements}

* 由[!DNL Sales Connect Salesforce]管理员安装的[!DNL Salesforce]包

* 已安装[!UICONTROL Push to Sales Connect]按钮以列出[!DNL Salesforce]管理员的视图

* 与[!DNL Salesforce]建立的[!DNL Sales Connect]连接用于发出推送的用户

## 操作方法 {#how-to}

1. 单击&#x200B;**[!UICONTROL Lead/Contact]**&#x200B;中的[!DNL Salesforce]选项卡。
1. 切换到[!DNL Sales Connect]按钮旁边要推送到[!UICONTROL Go]的列表视图。
1. 单击 **[!UICONTROL Go]**。
1. 选择您要推送至推播的所有潜在客户/联系人。
1. 选择 **[!UICONTROL Push to MSE]**。
1. 将出现一个新窗口，验证您要推移的潜在客户/联系人的数量。 选择 **[!UICONTROL Proceed to Group]**。[!DNL Sales Connect]不会推送任何在[!UICONTROL Email Opt Out]中标记为[!DNL Salesforce]或在[!UICONTROL Unsubscribed]中标记为[!DNL Sales Connect]的联系人。

   >[!NOTE]
   >
   >[!DNL Sales Connect]将这个标题为“SFDC-...”的群组添加到[Web应用程序](https://toutapp.com/login)上的“关系”页面。

1. 选择&#x200B;**[!UICONTROL Email Entire Group]**&#x200B;以发送此群电子邮件。
