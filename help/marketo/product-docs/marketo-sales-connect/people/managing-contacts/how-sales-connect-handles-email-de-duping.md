---
unique-page-id: 14352514
description: 了解Sales Connect如何处理电子邮件重复数据消除。 了解同步时如何合并或处理重复的联系人。
title: Sales Connect 如何处理电子邮件重复数据删除
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/gO6I2rCotAEDOGQNdRleeJbqMIix1wQizZe84JZSLPs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 6%

---

# [!DNL Sales Connect]如何处理电子邮件重复数据删除 {#how-sales-connect-handles-email-de-duping}

当您[将CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)文件上传到[!DNL Sales Connect]时，我们在导入之前合并CSV中的所有类似联系人。

我们根据相似的电子邮件地址来执行此操作。 因此，如果有两个相同的电子邮件地址，我们会将其合并为一个联系人。

如果您稍后尝试手动添加/上传同一联系人，则不会将其合并。

如果尝试添加数据库中已存在的联系人，我们将阻止您添加该联系人。
