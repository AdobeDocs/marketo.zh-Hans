---
unique-page-id: 14352514
description: Sales Connect如何处理电子邮件重复数据删除 — Marketo文档 — 产品文档
title: Sales Connect如何处理电子邮件重复数据删除
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Sales Connect如何处理电子邮件重复数据删除 {#how-sales-connect-handles-email-de-duping}

当您 [上传CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) 文件导入Sales Connect后，我们在导入之前将所有CSV中的类似联系人合并。

我们根据相似的电子邮件地址来执行此操作。 因此，如果有两个相同的电子邮件地址，我们会将其合并为一个联系人。

如果您稍后尝试手动添加/上传同一联系人，则不会合并该联系人。

如果尝试添加数据库中已存在的联系人，我们将阻止您添加该联系人。
