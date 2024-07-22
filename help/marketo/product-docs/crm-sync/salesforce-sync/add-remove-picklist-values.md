---
unique-page-id: 4719312
description: 添加/删除选取列表值 — Marketo文档 — 产品文档
title: 添加/删除选取列表值
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# 添加/删除选取列表值 {#add-remove-picklist-values}

以下是有关在Salesforce中添加和删除选择列表值的一些注意事项。

## 添加选取列表值 {#adding-picklist-values}

1. 如果在Salesforce中为选择列表字段类型添加了其他值，您将收到一个[通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"}，用于标识将影响哪些表单。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 转到表单编辑器，然后[将附加值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"}添加到您的建议列表中。

## 删除选择列表值 {#remove-picklist-values}

从Salesforce中的字段删除选择列表值后，您必须从托管此字段的所有表单中手动删除此值。

>[!NOTE]
>
>如果Salesforce中的潜在客户字段和联系人字段的值不同，则通用值将可用于Marketo Engage。

如果Salesforce中的潜在客户字段和联系人字段的值不同：

1. 在SFDC中向选择列表添加附加值将收到通知。
1. 通知会告诉您它在何处使用。 如果需要，您现在可以将此新值添加为表单上的选项。

如果SFDC潜在客户的选择列表与SFDC联系人的选择列表的值不同，则公用值将用作表单中的默认值选项。

如果从选取列表中删除某个值，则必须将其作为选项从表单中手动删除。
