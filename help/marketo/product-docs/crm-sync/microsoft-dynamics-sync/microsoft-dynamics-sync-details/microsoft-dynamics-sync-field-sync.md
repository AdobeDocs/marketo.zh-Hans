---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs —— 产品文档
title: Microsoft Dynamics Sync —— 字段同步
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Microsoft Dynamics同步：字段同步 {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

Marketo到Dynamics同步功能非常强大。 下面是详细信息。

## 字段详细信息如何在两个系统之间保持同步？ {#how-are-field-details-kept-in-sync-between-the-two-systems}

对于潜在客户和联系人实体，同步是双向的。 如果您在Dynamics中对潜在客户或联系人或Marketo中的人员进行了更改，您的更新将反映在两个系统中。

对于帐户、用户、机会、团队和自定义实体，同步是单向的：Marketo的动态。 如果您在Dynamics中对这些实体进行了更改，您的更新将反映在Marketo中。

## 如果同时对两个系统中的同一字段进行更改，该怎么办？ （数据冲突） {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

尽管这很少见，但Marketo将赢得人（线索）,Dynamics将赢得人脉。 这是因为我们认为营销部门对于人具有权威性，而官方的联系记录系统在销售(CRM)部门。 对于单向同步实体，Dynamics将始终获胜。

## 我是否可以使用Marketo在Dynamics中创建字段？ {#can-i-create-a-field-in-dynamics-using-marketo}

否，当前不支持。

## 我在动态网创建了一个字段。 能否将其同步到Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

是的，只要您 [的同步用户](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 在Dynamics中有权访问该字段，您就可以同步该字段。

哪些字段将同步到Marketo?

您可以 [在设置过程中选择要同步](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) 的字段。

## 如果我需要在Marketo和Dynamics同步后添加自定义字段，该怎么办？ {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

您可以随时添加字段，并期望数据从Dynamics刷新到Marketo。 有关 [详细信息，请参阅将快速同步与Microsoft Dynamics结合使用](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) 。

>[!NOTE]
>
>**相关文章**
>
>* [将快速同步与Microsoft Dynamics用于新的自定义字段](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



