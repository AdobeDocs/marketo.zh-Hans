---
unique-page-id: 2951640
description: 使用有趣的时刻 — Marketo文档 — 产品文档
title: 使用有趣的时刻
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# 使用有趣的时刻 {#using-interesting-moments}

有趣的时刻是通过Marketo Sales Insight应用程序与您的销售团队进行沟通的关键。

>[!AVAILABILITY]
>
>这些功能可供Marketo Sales Insight和 [Marketo Sales连接](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) 仅限客户。

## 什么是一个有趣的时刻？ {#what-is-an-interesting-moment}

由你来决定！ 您可以决定哪些信息与您的销售团队相关。 您的销售团队可能想知道销售线索何时出现：

* 访问您网站上的定价页面
* 单击新产品公告电子邮件中的链接
* 请求产品演示

## 我该如何创造一个有趣的时刻呢？  {#how-do-i-create-an-interesting-moment}

1. 选择 [智能营销活动](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)，最好是您的销售团队觉得有意思的一个，如果触发。

   ![](assets/using-interesting-moments-1.png)

1. 拖动到 **有趣的时刻** 流程步骤。

   ![](assets/using-interesting-moments-2.png)

1. 选择 **type** （电子邮件、里程碑或Web）。

   ![](assets/using-interesting-moments-3.png)

1. 在 **描述** 解释此操作重要原因的字段。

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo还将添加发生的日期以及添加有趣时刻的方式（即潜在客户操作>流程步骤、SOAP API）。

## 这怎么会更有趣呢？  {#how-can-this-get-even-more-interesting}

令牌！ 将它们添加到描述字段中，以便为您的销售团队提供更具体的信息，例如商机所打开电子邮件的主题行或发送者。 查看哪些令牌可用于中 [有趣时刻的令牌](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) 术语表。

>[!TIP]
>
>从五个有趣的时刻开始，然后与您的销售团队合作，以确定他们感兴趣的信息。

## Marketo中一个有趣的时刻是什么样的？  {#what-does-an-interesting-moment-look-like-in-marketo}

有趣的时刻将显示在 [商机的活动日志](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## 在Salesforce中，一个有趣的时刻是什么样的？  {#what-does-an-interesting-moment-look-like-in-salesforce}

一旦您 [已安装Marketo销售分析应用程序](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)，可在lead 、 contact 、 account或opportunity页面上显示有趣的时刻。 它们还会显示在Lead Feed 、 Best Bets和Watch List的Sales Insight仪表板中。

![](assets/using-interesting-moments-6.png)

## Salesforce1中一个有趣的时刻是什么样的？ {#what-does-an-interesting-moment-look-like-in-salesforce-1}

安装或更新Marketo Sales Insight for Salesforce1后，潜在客户的相关链接下将显示有趣的时刻。

![](assets/using-interesting-moments-7.png)

## 订阅有趣的时刻 {#subscribe-to-interesting-moments}

您可以通过单击“有趣的时刻”选项卡或“潜在客户源”中的“订阅”按钮来订阅“有趣的时刻”。 以下步骤对两者都是相同的。

1. 单击“订阅”图标。 然后，您将导航到Email Subscribe选项卡。

1. 您可以根据“名称”、“帐户”、“类型”或“描述”选择要接收的电子邮件警报类型。

1. 选择要将警报发送给（您自己/团队成员）的电子邮件地址

1. 单击 **订阅**.

>[!NOTE]
>
>在订阅有趣时刻类型或描述时，用户将在触发与该类型或描述匹配的有趣时刻时收到其拥有的人员（潜在客户/联系人）的电子邮件通知。

![](assets/using-interesting-moments-8.png)
