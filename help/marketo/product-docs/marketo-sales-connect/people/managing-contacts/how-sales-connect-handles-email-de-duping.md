---
unique-page-id: 14352514
description: Sales Connect如何处理电子邮件去重复处理 — Marketo文档 — 产品文档
title: Sales Connect如何处理电子邮件去重复
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Sales Connect如何处理电子邮件去重复 {#how-sales-connect-handles-email-de-duping}

当你 [上传CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) 文件到Sales Connect中时，在导入开始之前，我们会在CSV中合并所有类似的联系人。

我们根据相似电子邮件地址执行此操作。 因此，如果有两个相同的电子邮件地址，我们会将它们合并为一个联系人。

如果您稍后尝试手动添加/上传同一联系人，我们将不会合并该联系人。

如果您尝试添加数据库中已有的联系人，我们将阻止您添加该联系人。
