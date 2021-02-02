---
unique-page-id: 10095307
description: 电子邮件地址的自定义同步筛选器规则- Marketo Docs —— 产品文档
title: 电子邮件地址的自定义同步筛选器规则
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# 电子邮件地址{#custom-sync-filter-rules-for-an-email-address}的自定义同步过滤规则

要阻止同步没有电子邮件地址的记录，请遵循以下规则。

* 创建潜在客户或更新潜在客户的电子邮件地址字段时，检查潜在客户是否有电子邮件地址，如果有，将“同步到Mkto”更改为&#x200B;**True**。 否则，更改为&#x200B;**False**

* 创建联系人或更新联系人的电子邮件地址字段时，检查联系人是否有电子邮件地址，如果有，将“同步”更改为&#x200B;**True**，并在帐户记录中将“同步”更改为&#x200B;**True**。 否则，更改为&#x200B;**False**

* 更新联系人的公司名称(parentcustomerid)字段后，检查联系人的“同步到Mkto”字段是否为真。 如果是，则还将帐户上的“同步到Mkto”更改为&#x200B;**True**
* 当业务机会的潜在客户（客户id）字段或联系人（父代联系人）字段更新时，检查帐户的“与Mkto的同步”字段是否为真，或者联系人的“与Mkto的同步”字段是否为真。 如果是，则还应将机会上的“同步到Mkto”更改为&#x200B;**True**
