---
unique-page-id: 2360423
description: 在收入周期模型 — Marketo Docs — 产品文档中查找所有潜在客户
title: 在收入周期模型中查找所有潜在客户
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
translation-type: tm+mt
source-git-commit: c1b2a5966da3bda18a2ccaab9b348296ba1d7bfd
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# 在收入周期模型{#find-all-leads-in-a-revenue-cycle-model}中查找所有潜在客户

通过使用智能列表，您可以轻松找到收入周期模型的所有成员。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 选中智能列表后，单击&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. 找到收入模型&#x200B;**的**&#x200B;成员过滤器，并将其拖入画布中。

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. 选择&#x200B;**Model**。

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   这将使您获得该模型中的所有潜在客户，而不管是哪个阶段。 通常，您需要特定的舞台。 请改用以下筛选器。

1. 找到&#x200B;**收入阶段**&#x200B;过滤器并将其拖入画布。

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. 选择&#x200B;**Stage**。

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. 转到&#x200B;**Leads**&#x200B;选项卡以视图结果。

   ![](assets/2.png)

   >[!TIP]
   >
   >您不需要两个过滤器，只需选择所需的。 我们只是向你们展示，要彻底。

   >[!CAUTION]
   >
   >如果潜在客户的阶段在最初创建潜在客户时由外部活动更改，则活动不会记录在数据库中。 这意味着智能列表过滤器不会包括潜在客户。
