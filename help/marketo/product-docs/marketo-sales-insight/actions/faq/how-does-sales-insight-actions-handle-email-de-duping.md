---
description: Sales Insight操作如何处理电子邮件重复数据消除 — Marketo文档 — 产品文档
title: Sales Insight操作如何处理电子邮件重复数据消除
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Sales Insight操作如何处理电子邮件重复数据消除？ {#how-does-sales-insight-actions-handle-email-de-duping}

当您 [上传CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) 将文件导入Sales Insight Actions中，我们会在导入之前将CSV中的所有类似联系人合并。

我们根据相似的电子邮件地址来执行此操作。 因此，如果有两个相同的电子邮件地址，我们会将其合并为一个联系人。

如果您稍后尝试手动添加/上传同一联系人，则不会将其合并。

如果尝试添加数据库中已存在的联系人，我们将阻止您添加该联系人。
