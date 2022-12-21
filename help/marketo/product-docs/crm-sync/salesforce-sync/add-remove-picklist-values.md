---
unique-page-id: 4719312
description: 添加/删除选取列表值 — Marketo文档 — 产品文档
title: 添加/删除选取列表值
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 添加/删除选取列表值 {#add-remove-picklist-values}

以下是有关在Salesforce中添加和删除挑库值的一些信息。

## 添加选取列表值 {#adding-picklist-values}

1. 如果在Salesforce中向挑选列表字段类型添加了额外值，您将收到 [通知](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) 确定将影响哪些表单。

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. 转到表单编辑器和 [添加附加值](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) 列出建议。

## 删除选取列表值 {#remove-picklist-values}

从Salesforce中的字段中删除选取列表值后，您必须从托管该字段的所有表单中手动删除此值。

>[!NOTE]
>
>如果Salesforce中的潜在客户字段和联系人字段具有不同的值，则通用的值将可在Marketo中使用。

如果Salesforce中的潜在客户字段和联系人字段具有不同的值：

1. 将SFDC中的附加值添加到选取列表将收到通知。
1. 通知将告诉您该活动的使用位置。 现在，您可以根据需要将此新值作为选项添加到表单中。

如果SFDC潜在客户的挑选列表的值与SFDC联系人的挑选列表的值不同，则在表单中将使用常用值作为默认值选项。

如果从选取列表中删除某个值，则必须手动将其作为表单中的选项删除。
