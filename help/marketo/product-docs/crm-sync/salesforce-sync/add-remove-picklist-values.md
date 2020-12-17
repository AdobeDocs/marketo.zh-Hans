---
unique-page-id: 4719312
description: 添加／删除选择列表值- Marketo文档——产品文档
title: 添加／删除选择列表值
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 添加／删除选择列表值{#add-remove-picklist-values}

以下是有关在Salesforce中添加和删除选择列表值的一些信息。

## 添加Picklist值{#adding-picklist-values}

1. 如果在Salesforce中向选择列表字段类型添加了额外值，您将收到[通知](../../../product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md)，其中标识将影响哪些表单。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 转到表单编辑器并[将附加值](../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)添加到建议列表。

## 删除Picklist值{#remove-picklist-values}

从Salesforce中的字段删除选择列表值后，您必须从承载此字段的所有表单中手动删除此值。

>[!NOTE]
>
>如果Salesforce中的潜在客户字段和联系人字段具有不同的值，则通用值将可用于Marketo。

如果Salesforce中的潜在客户字段和联系人字段具有不同的值：

1. 将SFDC中的附加值添加到选择列表将收到通知。
1. 通知将告诉您它的使用位置。 现在，您可以根据需要在表单上添加此新值作为选项。

如果SFDC潜在客户的选择列表的值与SFDC联系人的选择列表的值不同，则公用值将用作表单中的默认值选项。

如果从选择列表中删除某个值，则必须手动将其作为选项从表单中删除。
