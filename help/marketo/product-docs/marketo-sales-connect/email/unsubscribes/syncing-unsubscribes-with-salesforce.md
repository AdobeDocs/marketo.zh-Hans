---
unique-page-id: 14746188
description: 与Salesforce同步取消订阅 — Marketo文档 — 产品文档
title: 正在与Salesforce同步取消订阅
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 1%

---

# 正在与[!DNL Salesforce]同步取消订阅 {#syncing-unsubscribes-with-salesforce}

## 取消订阅同步到[!DNL Salesforce]的要求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必须启用取消订阅同步（用于夜间同步）
* 必须在[!DNL Salesforce]中安装选择退出字段
* [!DNL Sales Connect]中的人员记录必须具有[!DNL Salesforce] ID

**推送取消订阅**

在[!DNL Sales Connect]中收集取消订阅时，我们会将其实时推送到[!DNL Salesforce]，并更新您选择与之同步的任何一个选择退出字段。 如果您已禁用[!DNL Salesforce]同步，我们仍会将取消订阅推送到电子邮件选择退出。

**取消订阅同步**

启用取消订阅同步后（下面的步骤3），您将打开夜间同步。 同步在PST下午8:00左右每天执行一次。 它会将Marketo Sales中的所有取消订阅与Salesforce中的选择退出字段双向同步。

## 配置取消订阅同步到[!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

用户可以决定是希望与Marketo也可以同步的标准电子邮件选择退出字段同步其取消订阅，还是可以与Marketo销售人员选择退出字段同步，以便区分销售人员取消订阅和营销人员取消订阅。

1. 转到[Web应用程序](https://toutapp.com/login)，单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-1.png)

1. 在[!UICONTROL Admin Settings]下，选择&#x200B;**[!UICONTROL Unsubscribes]**。

   ![](assets/two-2.png)

1. 单击&#x200B;**[!UICONTROL Syncing to Salesforce]**，然后启用夜间同步。

   ![](assets/three-2.png)

1. 选择要同步到的字段。

   ![](assets/4.png)

   | 字段 | 描述 |
   |---|---|
   | **[!UICONTROL Sync to Salesforce Opt Out field]** | 默认情况下处于选中状态，仅更新[!DNL Salesforce]选择退出字段。 |
   | **[!UICONTROL Sync to Marketo Sales Opt Out field]** | 如果要将销售和营销取消订阅分开，请选择此选项以更新其他[Marketo销售选择退出字段。](#msoo) |

## 在页面布局中安装选择退出字段 {#installing-the-opt-out-field-in-the-page-layout}

**电子邮件选择退出**

电子邮件选择退出是[!DNL Salesforce]中的标准字段，可从[!DNL Salesforce]安装。 您必须是[!DNL Salesforce]管理员才能安装它。

1. 转到[Salesforce.com](https://salesforce.com)并登录。

   ![](assets/five-1.png)

1. 单击您的用户名并选择&#x200B;**[!UICONTROL Setup]**。

   ![](assets/six-1.png)

1. 在快速查找框中，搜索Contact或Lead。 在此方案中，我们会将字段安装到联系人页面布局，但您希望为两个人员记录都安装。

   ![](assets/seven-1.png)

1. 选择 **[!UICONTROL Page Layouts]**。

   ![](assets/eight-1.png)

1. 选择您要添加该字段的页面布局旁的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/nine.png)

1. 选择 **[!UICONTROL Fields]**。

   ![](assets/ten.png)

1. 将[!UICONTROL Email Opt Out]拖放到页面布局中。

   ![](assets/11.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/twelve.png)

## Marketo销售人员选择退出 {#marketo-sales-opt-out}

Marketo销售人员选择退出字段是一个自定义字段，适用于已安装Marketo [!DNL Sales Connect]自定义项的用户。

成功将Marketo [!DNL Sales Connect]自定义项安装到[!DNL Salesforce]中后，您将会看到可供您使用的Marketo销售人员选择退出字段。
