---
unique-page-id: 557339
description: 查找并合并重复人员 — Marketo Docs — 产品文档
title: 查找并合并重复人
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 查找并合并重复人{#find-and-merge-duplicate-people}

Marketo在新人进入系统时自动去重复。 但是，您的CRM可能最初已将重复发送到Marketo。 下面介绍如何将它们合并。

>[!NOTE]
>
>Marketo不会针对Salesforce或Microsoft Dynamics同步或手动输入人员时自动进行重复数据消除。

>[!PREREQUISITES]
>
>查找和合并重复将涉及使用[内置/系统智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)。

## 查找重复{#find-duplicates}

1. 转到&#x200B;**Database**&#x200B;区域。

   ![](assets/db.png)

   >[!CAUTION]
   >
   >如果您使用Salesforce人员帐户，在Marketo中合并人员可能不起作用。 如果可能，请在Salesforce中合并记录。

1. 选择&#x200B;**可能的重复**&#x200B;系统智能列表，然后单击&#x200B;**人物**&#x200B;选项卡。

   ![](assets/two.png)

   >[!NOTE]
   >
   >您还可以[查找具有自定义逻辑的重复人员](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md)。

## 手动合并人员{#merge-people-manually}

>[!CAUTION]
>
>合并人员时，如果失去的人有Marketo自定义对象，它将&#x200B;**不**&#x200B;重新关联到获胜的人。 请在执行合并之前重新为自定义对象创建父级。

1. 按住Ctrl/Cmd并单击，选择重复，然后单击&#x200B;**合并人员**。

   ![](assets/three.png)

   >[!TIP]
   >
   >您可以为同一人拥有两个或多个重复 — 同时选择所有这些属性。

1. 您将看到&#x200B;_不_&#x200B;匹配的记录之间的值。 选择要保留的值。 完成后，单击&#x200B;**合并**。 如果不需要任何一个值，可以选中&#x200B;**Custom**&#x200B;并输入您选择的值。

   ![](assets/four.png)

   >[!NOTE]
   >
   >手动合并人员时，第一个选定的人将是“获胜者”。 因此，在“人员”选项卡中，如果您正在合并记录ID 198和199，而您恰巧先单击199, 199将是合并人员的记录ID。 如果合并了两个以上的记录，则这也适用。

   >[!TIP]
   >
   >合并比删除更好。 您将保留所有历史记录（页面访问、链接点击、电子邮件打开、表单填充等）。

## Salesforce中的效果{#effect-in-salesforce}

如果您有Salesforce集成，则有一些关于Salesforce中合并潜在客户效果的说明。

* 如果仅合并Lead或仅合并Contact，则它们会按照常规Salesforce规则合并。
* 将Lead和Contacts合并在一起时，所有Lead在合并每个普通Salesforce规则之前都会转换为Contacts。

有关合并潜在客户或联系人时Salesforce行为的具体信息，请检查以下Salesforce文档:

* [合并重复潜在客户](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [合并重复联系人](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## 批量合并{#bulk-merging}

如果手动合并的重复过多，请联系您的客户成功经理以讨论您的选择。

超级！ 如果您连接到CRM，则记录将按照以下规则合并到该处。
