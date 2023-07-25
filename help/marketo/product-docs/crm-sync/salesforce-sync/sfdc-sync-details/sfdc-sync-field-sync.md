---
unique-page-id: 2953461
description: SFDC同步 — 字段同步 — Marketo文档 — 产品文档
title: SFDC同步 — 字段同步
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# SFDC同步：字段同步 {#sfdc-sync-field-sync}

Marketo从Salesforce同步字段信息。 详情如下。

## 哪些字段已同步？ {#which-fields-are-synced}

我们同步SFDC中的大多数标准字段以及同步用户有权查看的任何自定义字段。

## 如何确定Marketo中的记录是Salesforce中的潜在客户还是联系人？ {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Marketo中有一个名为SFDC类型的字段。 它有三个可能的值：潜在客户、联系人或为空。 如果为空，则表示此Marketo潜在客户在SFDC中不存在。

## 如何确定是否在SFDC中删除了潜在客户或联系人？ {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Marketo中有一个名为SFDC isDeleted的字段。 如果该值为true，则潜在客户已在SFDC中删除。

## 如何确保在SFDC中添加的新字段也添加到Marketo？ {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>如果要在两个系统中都使用字段，请先在SFDC中创建该字段，它会自动同步到Marketo。

如果您在SFDC中添加了新字段，并且同步用户有权查看该字段，则该字段会自动添加到Marketo。

## 如果我更改SFDC中的字段标签，该怎么办？ {#what-if-i-change-a-field-label-in-sfdc}

更改SFDC中的字段标签不会影响Marketo中的字段标签。

## 如果我更改SFDC中的字段类型，该怎么办？ {#what-if-i-change-a-field-type-in-sfdc}

当您更改字段类型时，如果字段中的数据不匹配，Marketo会删除这些字段中的数据（但首先会显示警告）。 要保留数据，请确保在更改字段类型后导出数据并重新导入数据。

## 如果我在SFDC中更改API名称，该怎么办？ {#what-if-i-change-an-api-name-in-sfdc}

如果您更改SFDC中字段的API名称，则会在Marketo中创建一个新字段。

## 如果我在SFDC中添加新的选取列表值，会发生什么情况？ {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

如果在SFDC中将新的选择列表值添加到字段中，Marketo将向您发送通知。

## 自定义SFDC查找字段呢？ {#what-about-custom-sfdc-lookup-fields}

SFDC中的查找字段会同步ID，但不会同步引用的名称。

## SFDC公式字段怎么样？ {#what-about-sfdc-formula-fields}

公式字段会同步，但是，在更新之前，不会同步公式中引用的更新 [系统修改图章](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## 如果我从Salesforce中删除之前与Marketo同步的字段，会出现什么情况？ {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

如果删除SFDC中的字段，它不会自动删除Marketo中的字段，而只是停止同步。
