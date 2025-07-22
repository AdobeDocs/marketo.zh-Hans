---
unique-page-id: 2951640
description: 使用有趣的时刻 — Marketo文档 — 产品文档
title: 使用有趣的时刻
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 使用有趣的时刻 {#using-interesting-moments}

有趣的时刻是通过[!DNL Marketo Sales Insight]应用程序与您的销售团队进行沟通的关键。

>[!AVAILABILITY]
>
>这些仅对[!DNL Marketo Sales Insight]和[[!DNL Marketo Sales Connect]](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md)客户可用。

## 什么是一个有趣的时刻？ {#what-is-an-interesting-moment}

由你来决定！ 您可以决定哪些信息与您的销售团队相关。 您的销售团队可能想知道销售线索何时出现：

* 访问您网站上的定价页面
* 单击新产品公告电子邮件中的链接
* 请求产品演示

## 我该如何创造一个有趣的时刻？  {#how-do-i-create-an-interesting-moment}

1. 选择一个[智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)，最好是您的销售团队在触发时感兴趣的营销活动。

   ![](assets/using-interesting-moments-1.png)

1. 拖动到&#x200B;**[!UICONTROL Interesting Moments]**&#x200B;流程步骤上。

   ![](assets/using-interesting-moments-2.png)

1. 选择&#x200B;**类型** （[!UICONTROL Email]、[!UICONTROL Milestone]或[!UICONTROL Web]）。

   ![](assets/using-interesting-moments-3.png)

1. 在&#x200B;**[!UICONTROL Description]**&#x200B;字段中向您的销售团队写入一条消息，说明此操作重要的原因。

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo还将添加发生的日期以及添加有趣时刻的方式(即潜在客户操作>流程步骤、SOAP API)。

## 这怎么会更有趣呢？  {#how-can-this-get-even-more-interesting}

令牌！ 将它们添加到描述字段，以便为您的销售团队提供更具体的信息，例如商机所打开电子邮件的主题行或发送者。 查看哪些令牌可在[有趣时刻的令牌](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)术语表中使用。

>[!TIP]
>
>从五个有趣的时刻开始，然后与您的销售团队合作，以确定他们感兴趣的信息。

## 在Marketo中，一个有趣的时刻是什么样的？  {#what-does-an-interesting-moment-look-like-in-marketo}

有趣的时刻将显示在[潜在客户的活动日志](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)中。

![](assets/using-interesting-moments-5.png)

## 在[!DNL Salesforce]中，有趣的时刻是什么样的？  {#what-does-an-interesting-moment-look-like-in-salesforce}

在您[安装 [!DNL Marketo Sales Insight] 应用程序](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)后，潜在客户、联系人、客户或机会页面上将显示有趣的时刻。 它们还显示在潜在客户信息源[!DNL Sales Insight]和观察列表的[!DNL Best Bets]仪表板中。

![](assets/using-interesting-moments-6.png)

## 在[!DNL Salesforce1]中，有趣的时刻是什么样的？ {#what-does-an-interesting-moment-look-like-in-salesforce-1}

安装或更新[!DNL Marketo Sales Insight]的[!DNL Salesforce1]后，潜在客户的相关链接下将显示有趣的时刻。

![](assets/using-interesting-moments-7.png)

## 订阅有趣的时刻 {#subscribe-to-interesting-moments}

您可以通过单击“有趣的时刻”选项卡或“潜在客户”信息源中的[!UICONTROL Subscribe]按钮来订阅有趣的时刻。 以下步骤对两者相同。

1. 单击订阅图标。 随后将导航到Email Subscribe选项卡。

1. 您可以根据[!UICONTROL Name]、[!UICONTROL Account]、[!UICONTROL Type]或[!UICONTROL Description]选择要接收的电子邮件警报类型。

1. 选择要将警报发送给（您自己/团队成员）的电子邮件地址

1. 单击 **[!UICONTROL Subscribe]**。

>[!NOTE]
>
>在订阅有趣的时刻类型或描述时，用户将在触发与该类型或描述匹配的有趣时刻时收到其拥有的人员（潜在客户/联系人）的电子邮件通知。

![](assets/using-interesting-moments-8.png)
