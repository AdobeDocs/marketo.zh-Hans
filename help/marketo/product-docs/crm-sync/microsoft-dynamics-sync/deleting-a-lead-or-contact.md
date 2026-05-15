---
unique-page-id: 45417322
description: 了解在Microsoft Dynamics和Marketo之间如何删除商机和联系人。 根据需要使用Microsoft已删除标志和删除人员流程操作。
title: 删除潜在客户或联系人
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/4BwBuLQFJ2pRehuS8EqW-UrEcg5sVeqcstu3azh0NvQ
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 167
ht-degree: 5%

---

# 删除潜在客户或联系人 {#deleting-a-lead-or-contact}

关于删除[!DNL Microsoft Dynamics]中的潜在客户/联系人，有几点需要了解。

* Marketo不会仅因为潜在客户已在[!DNL Dynamics]中删除而自动删除人员。 相反，“Microsoft已删除”字段标志设置为true。 如果需要，您可以触发此字段以删除Marketo中的记录。

* “删除人员”流程操作：此操作仅删除Marketo中的人员（在Dynamics中用于同时删除人员的选项不可用）。

* 如果在Marketo中删除潜在客户（但不在[!DNL Dynamics]中），并且在该潜在客户在[!DNL Dynamics]中更新后，它将在Marketo中创建一个新人员（相同的电子邮件地址、新人员ID）。

* 如果在[!DNL Dynamics]中删除潜在客户（但未在Marketo中删除），然后通过“将人员同步到Microsoft”流程操作运行，则它将在[!DNL Dynamics]中创建新的潜在客户。
