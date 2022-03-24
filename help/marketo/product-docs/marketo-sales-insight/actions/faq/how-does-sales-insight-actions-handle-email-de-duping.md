---
description: Sales Insight Action如何处理电子邮件消除重复 — Marketo文档 — 产品文档
title: Sales Insight Action如何处理电子邮件消除重复
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Sales Insight Action如何处理电子邮件消除重复？ {#how-does-sales-insight-actions-handle-email-de-duping}

当你 [上传CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) 文件到Sales Insight Actions中时，我们会在导入开始之前，在CSV中合并所有类似的联系人。

我们根据相似电子邮件地址执行此操作。 因此，如果有两个相同的电子邮件地址，我们会将它们合并为一个联系人。

如果您稍后尝试手动添加/上传同一联系人，我们将不会合并该联系人。

如果您尝试添加数据库中已有的联系人，我们将阻止您添加该联系人。
