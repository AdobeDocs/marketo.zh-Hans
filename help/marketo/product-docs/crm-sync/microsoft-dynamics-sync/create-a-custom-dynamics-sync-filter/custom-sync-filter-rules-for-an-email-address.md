---
unique-page-id: 10095307
description: 了解如何在Dynamics中为电子邮件地址设置自定义同步筛选规则。 根据潜在客户或联系人是否有电子邮件，使用工作流将同步设置为Mkto。
title: 电子邮件地址的自定义同步过滤规则
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 7%

---

# 电子邮件地址的自定义同步过滤规则 {#custom-sync-filter-rules-for-an-email-address}

要防止同步没有电子邮件地址的记录，请遵循这些规则。

* 在创建潜在客户或更新潜在客户的电子邮件地址字段时，检查潜在客户是否有电子邮件地址，如果有，则将“同步到Mkto”更改为&#x200B;**[!UICONTROL True]**。 否则更改为&#x200B;**[!UICONTROL False]**

* 创建联系人或更新联系人的电子邮件地址字段时，检查联系人是否有电子邮件地址，如果有，在“帐户”记录上将“同步到Mkto”更改为&#x200B;**[!UICONTROL True]**，并将“同步到Mkto”更改为&#x200B;**[!UICONTROL True]**。 否则，将更改为&#x200B;**[!UICONTROL False]**

* 更新联系人的“公司名称”(parentcustomerid)字段后，检查联系人的“同步到Mkto”字段是否为true。 如果是，也将&#x200B;**[!UICONTROL True]**&#x200B;帐户上的Sync to更改为Mkto
* 更新商机的潜在客户(customerid)字段或联系人(parentcontactid)后，检查帐户的“同步到Mkto”字段是否为true，或联系人的“同步到Mkto”字段是否为true。 如果是，也将Opportunity上的Sync更改为Mkto更改为&#x200B;**[!UICONTROL True]**
