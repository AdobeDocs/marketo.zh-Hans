---
unique-page-id: 4719283
description: 了解Salesforce同步- Marketo文档——产品文档
title: 了解Salesforce同步
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# 了解Salesforce同步 {#understanding-the-salesforce-sync}

Marketo和Salesforce一起吃豆子和胡萝卜。 我们可同步您的销售和营销数据。

## 同步的工作方式 {#how-sync-works}

Marketo每天都与Salesforce同步。 每次同步都需要一些时间，然后暂停5分钟，然后再次开始。

>[!NOTE]
>
>您订阅中的第一次同步可能需要数小时甚至数天，因为Marketo正在从Salesforce复制整个数据库。 之后，每次同步通常需要几秒钟或几分钟，并且只同步已更改的数据。

![](assets/sync-illustration.png)

Salesforce和Marketo之间的同步仅针对潜在客户、联系人和Salesforce活动是双向的。 在这些情况下，只要您在Salesforce或Marketo中进行更改，您的更新就会反映在这两个系统中。 所有其他同步仅从Salesforce到Marketo。 单击以下链接可了解每个链接的详细信息。

## Marketo和Salesforce之间同步了什么？ {#what-is-synced-between-marketo-and-salesforce}

* [潜在客户](sfdc-sync-details/sfdc-sync-lead-sync.md)
* [联系人](sfdc-sync-details/sfdc-sync-contact-sync.md)
* [帐户](sfdc-sync-details/sfdc-sync-account-sync.md)
* [用户](sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [机会](sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce活动](sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [自定义对象](sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [活动](sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>您 [在Marketo中为Salesforce输入的凭据](setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ，用于同步数据。 将仅包含这些凭据有权访问的数据。

Salesforce同步有许多细微差别和功能。 查看SFDC同步详细信 [息部分的详细信息](http://docs.marketo.com/display/docs/sfdc+sync+details)。

>[!NOTE]
>
>**相关文章**
>
>* [Salesforce同步设置](http://docs.marketo.com/display/docs/setup)
>* [SFDC同步详细信息](http://docs.marketo.com/display/docs/sfdc+sync+details)

>



Marketo与Salesforce的同步是世界上同类产品中最强大的。 这感觉就像是魔法——一个变化已经发生，另一个系统很快就会更新。