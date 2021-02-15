---
unique-page-id: 14352514
description: Sales Connect如何处理电子邮件消除重复 — Marketo Docs — 产品文档
title: Sales Connect如何处理电子邮件消除重复
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Sales Connect如何处理电子邮件消除重复{#how-sales-connect-handles-email-de-duping}

将CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)文件上载到Sales Connect中后，在导入之前，我们会在CSV中合并所有类似的联系人。[

我们根据类似的电子邮件地址执行此操作。 因此，如果有两个相同的电子邮件地址，我们会将它们合并为一个联系人。

如果您稍后尝试手动添加/上传同一联系人，我们将不会合并它。

如果您尝试添加已在数据库中的联系人，我们将阻止您添加该联系人。
