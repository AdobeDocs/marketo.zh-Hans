---
unique-page-id: 10095307
description: 电子邮件地址的自定义同步筛选规则 — Marketo文档 — 产品文档
title: 电子邮件地址的自定义同步筛选规则
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# 电子邮件地址的自定义同步筛选规则 {#custom-sync-filter-rules-for-an-email-address}

要防止同步没有电子邮件地址的记录，请遵循这些规则。

* 在创建潜在客户或更新该潜在客户的电子邮件地址字段时，检查该潜在客户是否具有电子邮件地址，如果具有，则将“同步”更改为“Mkto” **True**. 否则更改为 **假**

* 创建联系人或更新联系人的电子邮件地址字段时，检查联系人是否有电子邮件地址，如果有，则将“同步”更改为“Mkto” **True** 并将同步更改为Mkto **True** 在帐户记录上。 否则，将更改为 **假**

* 更新联系人的“公司名称”(parentcustomerid)字段后，检查联系人的“同步到Mkto”字段是否为true。 如果是，则将帐户上的Sync更改为Mkto **True** 另外
* 更新商机的潜在客户(customerid)字段或联系人(parentcontactid)后，检查帐户的“同步到Mkto”字段是否为true，或联系人的“同步到Mkto”字段是否为true。 如果是，则将机会上的同步更改为Mkto **True** 另外
