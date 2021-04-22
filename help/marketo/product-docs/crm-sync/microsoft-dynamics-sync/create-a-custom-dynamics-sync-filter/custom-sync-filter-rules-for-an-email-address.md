---
unique-page-id: 10095307
description: 电子邮件地址的自定义同步筛选器规则 — Marketo Docs — 产品文档
title: 电子邮件地址的自定义同步筛选器规则
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# 电子邮件地址{#custom-sync-filter-rules-for-an-email-address}的自定义同步筛选器规则

要阻止没有电子邮件地址的记录同步，请遵循以下规则。

* 创建潜在客户或更新潜在客户的电子邮件地址字段时，检查潜在客户是否有电子邮件地址，如果有，将“同步到Mkto”更改为&#x200B;**True**。 否则，更改为&#x200B;**False**

* 创建联系人时，或当更新联系人的电子邮件地址字段时，检查该联系人是否有电子邮件地址，如果有，将“同步”更改为&#x200B;**True**，并将“帐户记录”中的“同步”更改为&#x200B;**True**。 否则，更改为&#x200B;**False**

* 更新联系人的公司名称(parentcustomerid)字段时，检查联系人的“同步到Mkto”字段是否为true。 如果是，则还将帐户上的“同步到Mkto”更改为&#x200B;**True**
* 当业务机会的潜在客户(customerid)字段或联系人(parentcontact)字段更新时，检查帐户的“同步到Mkto”字段是否为真，或者联系人的“同步到Mkto”字段是否为真。 如果是，则也将Opportunity的Sync更改为Mkto，为&#x200B;**True**
