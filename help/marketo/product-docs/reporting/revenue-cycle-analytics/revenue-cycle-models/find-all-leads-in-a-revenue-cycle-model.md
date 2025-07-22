---
unique-page-id: 2360423
description: 在收入周期模型中查找所有潜在客户 — Marketo文档 — 产品文档
title: 在收入周期模型中查找所有潜在客户
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# 在收入周期模型中查找所有潜在客户 {#find-all-leads-in-a-revenue-cycle-model}

通过使用智能列表，您可以轻松查找收入周期模型的所有成员。

>[!PREREQUISITES]
>
>[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 选定智能列表后，单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. 找到&#x200B;**[!UICONTROL Member of Revenue Model]**&#x200B;筛选器并将其拖到画布中。

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. 选择&#x200B;**[!UICONTROL Model]**。

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   这将获得该模型中的所有商机，无论处于哪个阶段。 通常您需要一个特定的阶段。 请改用以下过滤器。

1. 找到&#x200B;**[!UICONTROL Revenue Stage]**&#x200B;筛选器并将其拖到画布中。

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. 选择&#x200B;**[!UICONTROL Stage]**。

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. 转到&#x200B;**[!UICONTROL Leads]**&#x200B;选项卡以查看结果。

   ![](assets/2.png)

   >[!TIP]
   >
   >您不需要两个过滤器，只需选择所需的过滤器即可。 我们只是向您展示两者，以便进行彻底的检查。

   >[!CAUTION]
   >
   >如果在最初创建商机期间外部营销活动更改了商机的阶段，则活动不会记录到数据库中。 这意味着智能列表过滤器将不包含潜在客户。
