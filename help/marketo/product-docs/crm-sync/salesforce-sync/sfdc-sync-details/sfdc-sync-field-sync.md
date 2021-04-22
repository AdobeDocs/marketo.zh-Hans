---
unique-page-id: 2953461
description: SFDC同步 — 字段同步 — Marketo Docs — 产品文档
title: SFDC同步 — 字段同步
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# SFDC同步：字段同步{#sfdc-sync-field-sync}

Marketo同步来自Salesforce的字段信息。 下面是详细信息。

## 哪些字段已同步？{#which-fields-are-synced}

我们同步SFDC中的大多数标准字段和同步用户有权查看的任何自定义字段。

## 您如何确定Marketo中的记录是Salesforce中的潜在客户还是联系人？{#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

我们在Marketo中有一个名为SFDC类型的字段。 它有三个可能的值：领导，联系，或者是空的。 如果它为空，则表示此Marketo潜在客户在SFDC中不存在。

## 如何确定SFDC中是否删除了潜在客户或联系人？{#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

我们在Marketo中有一个名为SFDC isDeleted的字段。 如果值为true，则在SFDC中删除了潜在客户。

## 如何确保在SFDC中添加的新字段也添加到Marketo?{#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>如果您希望在两个系统中都有一个字段，请先在SFDC中创建它，它将自动同步到Marketo。

如果您在SFDC中添加了新字段，且同步用户有权查看该字段，它将自动添加到Marketo。

## 如果我更改了SFDC中的字段标签怎么办？{#what-if-i-change-a-field-label-in-sfdc}

在SFDC中更改字段标签不会影响Marketo中的字段标签。

## 如果我在SFDC中更改字段类型，该怎么办？{#what-if-i-change-a-field-type-in-sfdc}

更改字段类型时，如果字段中的数据不匹配，Marketo将删除这些字段中的数据（但首先显示警告）。 要保留数据，请务必在更改字段类型后导出并重新导入数据。

## 如果我在SFDC中更改API名称怎么办？{#what-if-i-change-an-api-name-in-sfdc}

如果在SFDC中更改字段的API名称，将在Marketo中创建新字段。

## 如果我在SFDC中添加新的选择列表值，会发生什么情况？{#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

如果在SFDC中向字段添加了新的选择列表值，Marketo将向您发送通知。

## 自定义SFDC查找字段如何？{#what-about-custom-sfdc-lookup-fields}

SFDC中的查找字段会同步ID，但不会同步引用的名称。

## SFDC公式字段如何？{#what-about-sfdc-formula-fields}

公式字段会同步，但是，在[系统模块图章](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US)有更新之前，不会同步对公式中引用的更新。

## 当我从Salesforce中删除之前与Marketo同步的字段时，会出现什么情况？{#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

如果您在SFDC中删除字段，它不会自动删除Marketo中的字段，它只会停止同步。
