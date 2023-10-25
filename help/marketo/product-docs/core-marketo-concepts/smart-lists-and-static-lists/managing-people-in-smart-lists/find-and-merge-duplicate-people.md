---
unique-page-id: 557339
description: 查找并合并重复人员 — Marketo文档 — 产品文档
title: 查找并合并重复的人员
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 查找并合并重复的人员 {#find-and-merge-duplicate-people}

当新人员进入Marketo Engage时，系统会自动删除重复项。 但是，您的CRM最初可能通过重复项发送。 下面是如何将它们合并的。

>[!CAUTION]
>
>合并人员是永久性的，没有“撤消”选项。

>[!PREREQUISITES]
>
>查找和合并重复项需要使用 [内置/系统智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo不会针对Salesforce或Microsoft Dynamics同步自动执行重复数据删除，或者在您手动输入人员时执行重复数据删除。

## 查找重复项 {#find-duplicates}

1. 转到 **[!UICONTROL 数据库]** 区域。

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >如果使用Salesforce人员帐户，则在Marketo中合并人员可能无法正常工作。 如果可能，请合并Salesforce中的记录。

1. 选择 **[!UICONTROL 可能的重复项]** 系统智能列表，然后单击 **[!UICONTROL 人员]** 选项卡。

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >您还可以 [使用自定义逻辑查找重复的人员](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## 手动合并人员 {#merge-people-manually}

>[!CAUTION]
>
>在合并人员时，如果失败人员具有Marketo自定义对象，则将 _非_ 重新关联到入选人员。 在执行合并之前，请重新为自定义对象添加父级。

1. 按住Ctrl/Cmd并单击以选择重复项，然后单击 **[!UICONTROL 合并人员]**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >您可以为同一人员创建两个或多个重复项 — 一次选择所有重复项。

1. 您将看到以下记录之间的值： _不要_ 匹配。 为每个字段选择要保留的值。 单击 **[!UICONTROL 合并]** 完成时。 如果您不希望获得这两个值，则可以选中 **[!UICONTROL 自定义]** 并输入您选择的值。

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >手动合并人员时，第一个被选中的人员将成为“入选者”。 在“人员”选项卡中，如果您要合并记录ID 198和199，并且碰巧首先单击199，则199将是合并人员的记录ID。 如果合并了两个以上的记录，这也适用。

   >[!TIP]
   >
   >合并总比删除好。 您将保留所有历史记录（页面访问次数、链接点击次数、电子邮件打开次数、表单填写次数等）。

## Salesforce中的效果 {#effect-in-salesforce}

如果您集成了Salesforce，下面是有关在Salesforce中合并潜在客户效果的一些注释。

* 当仅合并潜在客户或仅合并联系人时，它们会按照正常的Salesforce规则合并。
* 将Lead和Contacts合并在一起时，所有Lead在合并之前都会转换为Contacts，然后按照正常的Salesforce规则进行合并。

有关合并潜在客户或联系人时Salesforce行为的详细信息，请查看以下Salesforce文档：

* [合并重复的潜在客户](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US){target="_blank"}
* [合并重复的联系人](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US){target="_blank"}

## 批量合并 {#bulk-merging}

如果您有太多要手动合并的重复项，请联系Adobe客户团队（您的客户经理）以讨论您的选项。
