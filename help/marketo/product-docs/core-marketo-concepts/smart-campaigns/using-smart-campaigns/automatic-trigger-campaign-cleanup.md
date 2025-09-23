---
unique-page-id: 1147074
description: 自动触发营销活动清理 — Marketo文档 — 产品文档
title: 自动清理触发型营销活动
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 3%

---

# 自动清理触发型营销活动 {#automatic-trigger-campaign-cleanup}

Marketo提供了一项好的/免费的服务，用于停用已触发的“智能营销活动”，使其不再进行活动。 这可以提高整体系统性能并节省您的时间。

## 会发生什么？ {#what-happens}

每季度一次，Marketo会发现闲置6个月或更长时间（没有人员）的智能营销活动并将其停用。

## 你先通知我好吗？ {#will-you-notify-me-first}

当然！ 每季度一次，您会提前一周收到通知，显示我们计划停用的每个营销活动。

1. 单击&#x200B;**[!UICONTROL Notifications]**&#x200B;图标。

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. 单击&#x200B;**[!UICONTROL Idle Trigger Campaign Cleanup Scheduled]**。 然后单击&#x200B;**[!UICONTROL These Idle Trigger Campaigns will be deactivated]**&#x200B;链接。

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   您将看到一个计划取消激活的智能营销活动列表。

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## 将停用哪些营销活动？ {#which-campaigns-will-be-deactivated}

我们将仅取消激活已激活超过6个月但在此期间有0人符合条件的触发营销活动。

## 等等！ 不是此营销活动！ {#wait-not-this-campaign}

不必担心 — 任何Smart Campaign的时钟都可以通过以下方式重置：

* 符合营销活动资格的人员。
* 手动停用和重新激活营销活动。

两者都会重置6个月的计数器。

## 能否告知我哪些营销活动已停用？ {#will-you-let-me-know-which-campaigns-were-deactivated}

绝对 — 在原始通知发布一周后，我们将停用列出的营销活动（减去任何至少符合一个人条件或已停用/重新激活的营销活动），并发布确认通知。

1. 选择&#x200B;**[!UICONTROL Idle Trigger Campaign Cleanup Scheduled]**&#x200B;通知。 单击&#x200B;**[!UICONTROL These Idle Trigger Campaigns]**&#x200B;链接。

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. 您将看到已停用营销活动的列表。

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
