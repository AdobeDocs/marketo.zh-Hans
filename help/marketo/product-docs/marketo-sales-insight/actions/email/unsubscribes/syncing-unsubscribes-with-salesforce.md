---
description: 与Salesforce同步取消订阅 — Marketo文档 — 产品文档
title: 正在与Salesforce同步取消订阅
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 1%

---

# 正在与[!DNL Salesforce]同步取消订阅 {#syncing-unsubscribes-with-salesforce}

如果要使用Salesforce中的选择退出字段同步取消订阅，则可以使用Salesforce取消订阅同步。

## 取消订阅同步到Salesforce的要求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必须启用取消订阅同步（用于夜间同步）
* 必须在[!DNL Salesforce]中安装选择退出字段
* [!DNL Marketo Sales]中的人员记录必须具有[!DNL Salesforce] ID

**推送取消订阅**

在[!DNL Marketo Sales]中收集取消订阅时，我们会将其实时推送到[!DNL Salesforce]，并更新您选择与之同步的任何一个选择退出字段。 如果您已禁用[!DNL Salesforce]同步，我们仍会将取消订阅推送到电子邮件选择退出。

**取消订阅同步**

启用取消订阅同步后（下面的步骤3），您将启用夜间同步。 同步在PST下午8:00左右每天执行一次。 它会将Marketo Sales中的所有取消订阅与Salesforce中的选择退出字段双向同步。

>[!NOTE]
>
>取消订阅与Salesforce同步将同步取消订阅，但不会同步重新订阅。 如果要从Marketo Sales和Salesforce中删除取消订阅，请在Salesforce中取消选中取消订阅，然后在Marketo Sales中移除取消订阅。

## 配置取消订阅同步到[!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

用户可以决定是希望与Marketo也可以同步的标准电子邮件选择退出字段同步其取消订阅，还是可以与[!DNL Marketo Sales]选择退出字段同步，以便区分销售取消订阅和营销取消订阅。

1. 单击齿轮图标并选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. 在[!UICONTROL Admin Settings]下，选择&#x200B;**[!UICONTROL Unsubscribes]**。

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 单击&#x200B;**[!UICONTROL Integrations]**&#x200B;选项卡。 在[!UICONTROL Sync to Salesforce]下，启用夜间同步。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 选择要同步到的字段。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | 字段 | 描述 |
   |---|---|
   | **同步到[!DNL Salesforce]选择退出字段** | 默认情况下处于选中状态，仅更新[!DNL Salesforce]选择退出字段。 |
   | **同步到[!DNL Marketo Sales]选择退出字段** | 如果要将销售和营销取消订阅分开，请选择此选项以更新其他[[!DNL Marketo Sales] 选择退出字段。](#msoo) |

## 在页面布局中安装选择退出字段 {#installing-the-opt-out-field-in-the-page-layout}

**电子邮件选择退出**

电子邮件选择退出是[!DNL Salesforce]中的标准字段，可从[!DNL Salesforce]安装。 您必须是[!DNL Salesforce]管理员才能安装它。

1. 转到[Salesforce.com](https://salesforce.com)并登录。

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. 单击您的用户名并选择&#x200B;**[!UICONTROL Setup]**。

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. 在快速查找框中，搜索Contact或Lead。 在此方案中，我们会将字段安装到联系人页面布局，但您希望为两个人员记录都安装。

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. 选择 **[!UICONTROL Page Layouts]**。

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. 选择您要添加该字段的页面布局旁的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. 选择 **[!UICONTROL Fields]**。

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. 将[!UICONTROL Email Opt Out]拖放到页面布局中。

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo销售人员选择退出 {#marketo-sales-opt-out}

Marketo Sales Opt Out字段是一个自定义字段，适用于已从AppExchange[安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}的用户。

成功将Marketo Sales Insight包从AppExchange安装到Salesforce中后，您将会看到可用的Marketo Sales Opt Out字段。
