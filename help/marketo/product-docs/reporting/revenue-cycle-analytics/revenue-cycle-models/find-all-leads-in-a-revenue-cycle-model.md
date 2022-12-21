---
unique-page-id: 2360423
description: 在收入周期模型中查找所有潜在客户 — Marketo文档 — 产品文档
title: 在收入周期模型中查找所有潜在客户
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
source-git-commit: c1b2a5966da3bda18a2ccaab9b348296ba1d7bfd
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# 在收入周期模型中查找所有潜在客户 {#find-all-leads-in-a-revenue-cycle-model}

通过使用智能列表，您可以轻松找到收入周期模型的所有成员。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 选择智能列表后，单击 **智能列表** 选项卡。

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. 查找 **收入模型成员** 过滤并将其拖到画布中。

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. 选择 **模型**.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   这会得到模型中的所有潜在客户，无论是哪个阶段。 通常，您会想要一个特定的阶段。 请改用以下过滤器。

1. 查找 **收入阶段** 过滤并将其拖到画布中。

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. 选择 **阶段**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. 转到 **潜在客户** 选项卡查看结果。

   ![](assets/2.png)

   >[!TIP]
   >
   >您不需要同时使用这两个过滤器，只需选择所需的过滤器即可。 我们只是向你们展示，要彻底。

   >[!CAUTION]
   >
   >如果在最初创建潜在客户期间，外部营销活动更改了潜在客户的阶段，则活动不会记录到数据库中。 这意味着智能列表过滤器不会包含潜在客户。
