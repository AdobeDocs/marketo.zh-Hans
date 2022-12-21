---
unique-page-id: 10095307
description: 电子邮件地址的自定义同步过滤器规则 — Marketo文档 — 产品文档
title: 电子邮件地址的自定义同步过滤器规则
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# 电子邮件地址的自定义同步过滤器规则 {#custom-sync-filter-rules-for-an-email-address}

要阻止同步没有电子邮件地址的记录，请遵循以下规则。

* 创建潜在客户时或更新潜在客户的电子邮件地址字段时，检查潜在客户是否具有电子邮件地址，如果有，请将“同步到Mkto”更改为 **True**. 否则，请将 **False**

* 创建联系人或更新联系人的电子邮件地址字段后，请检查联系人是否具有电子邮件地址，如果有，请将“同步到Mkto”更改为 **True** 并将同步更改为Mkto **True** 在帐户记录中。 否则，请将 **False**

* 更新联系人的公司名称(parentcustomerid)字段后，检查联系人的同步到Mkto字段是否为true。 如果是，请将帐户上的“同步到Mkto”更改为 **True** 也
* 当业务机会的潜在客户（客户ID）字段或联系人（父代联系人）字段更新时，检查帐户的“同步到Mkto”字段是否为true，或联系人的“同步到Mkto”字段是否为true。 如果是，请在机会上将“同步到Mkto”更改为 **True** 也
