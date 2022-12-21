---
unique-page-id: 557339
description: 查找并合并重复人员 — Marketo文档 — 产品文档
title: 查找并合并重复人员
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 查找并合并重复人员 {#find-and-merge-duplicate-people}

Marketo会在新用户进入系统时自动删除重复项。 但是，您的CRM最初可能已将重复项发送到Marketo。 下面是如何合并它们。

>[!NOTE]
>
>Marketo不会针对Salesforce或Microsoft Dynamics同步或在您手动输入人员时自动消除重复数据。

>[!PREREQUISITES]
>
>查找和合并重复项将涉及使用 [内置/系统智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md).

## 查找重复项 {#find-duplicates}

1. 转到 **数据库** 的上界。

   ![](assets/db.png)

   >[!CAUTION]
   >
   >如果您使用Salesforce人员帐户，则合并Marketo中的人员可能不起作用。 如果可能，请合并Salesforce中的记录。

1. 选择 **可能的重复项** 系统智能列表并单击 **人员** 选项卡。

   ![](assets/two.png)

   >[!NOTE]
   >
   >您还可以 [使用自定义逻辑查找重复人员](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md).

## 手动合并人员 {#merge-people-manually}

>[!CAUTION]
>
>合并人员时，如果丢失的人员具有Marketo自定义对象，则会 **not** 重新关联到入选者。 在执行合并之前，请重新为自定义对象生成父项。

1. 按住Ctrl/Cmd并单击，以选择重复项，然后单击 **合并人员**.

   ![](assets/three.png)

   >[!TIP]
   >
   >同一人员可以有两个或多个重复项 — 一次选择所有重复项。

1. 您将看到这些记录之间的值 _不_ 匹配。 选择要保留的每个字段值。 单击 **合并** 完成时。 如果不需要任一值，可以检查 **自定义** 并输入您选择的值。

   ![](assets/four.png)

   >[!NOTE]
   >
   >手动合并人员时，第一个选定的人员将是“入选者”。 因此，在“人员”选项卡中，如果您将记录ID合并到198和199，并且您恰巧先单击199，则199将是合并后人员的记录ID。 如果合并了两个以上的记录，则也适用这一点。

   >[!TIP]
   >
   >合并好过删除。 您将保留所有历史记录（页面访问、链接点击、电子邮件打开、表单填充等）。

## 在Salesforce中的影响 {#effect-in-salesforce}

如果您集成了Salesforce，则有关Salesforce中合并潜在客户的效果的一些说明。

* 仅合并潜在客户或仅合并联系人时，它们会按照常规的Salesforce规则进行合并。
* 将潜在客户和联系人合并在一起时，所有潜在客户在按照常规Salesforce规则合并之前都会转换为联系人。

有关合并潜在客户或联系人时Salesforce行为的具体说明，请查看以下Salesforce文档：

* [合并重复的潜在客户](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [合并重复的联系人](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## 批量合并 {#bulk-merging}

如果手动合并的重复项过多，请联系您的客户成功经理来讨论您的选项。

超级！ 如果您连接到CRM，则根据以下规则，记录将合并到该处。
