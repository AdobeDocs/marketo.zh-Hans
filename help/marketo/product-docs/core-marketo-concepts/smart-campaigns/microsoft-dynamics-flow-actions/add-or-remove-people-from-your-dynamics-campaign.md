---
description: 从Dynamics Campaign中添加或移除人员 — Marketo文档 — 产品文档
title: 在Dynamics Campaign中添加或删除人员
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 在Dynamics Campaign中添加或删除人员 {#add-or-remove-people-from-your-dynamics-campaign}

## 添加到Dynamics Campaign {#add-to-dynamics-campaign}

此流程步骤可用于Marketo Smart Campaigns，以将人员添加为Microsoft营销活动中的潜在客户或联系人。 如果Dynamics中尚不存在潜在客户，则会自动将其同步到并添加到营销活动中。

>[!NOTE]
>
>此流程操作仅适用于触发营销活动。

在智能营销活动中，查找并选择要将人员添加到的动态营销活动。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果在营销活动列表中看不到Dynamics营销活动：
>
>* 确保Campaign同步正常运行
>* 该营销活动在Microsoft Dynamics中处于非活动状态

系统会自动创建特定于营销活动的静态营销列表，每个列表都用于潜在客户和联系人，以将该人员添加到。 这是一次性操作，后续同步到营销活动时，将使用相同的营销列表。 静态营销列表名称采用的命名标准为 `Mkto-leads-<uniqueID>` 潜在客户和 `Mkto-contacts-<uniqueID>` 用于联系人。

将这些Marketo生成的营销列表与其他营销活动关联可能会导致混淆行为。 例如：添加到一个营销活动也会导致添加到第二个营销活动。 同样，也不建议在Dynamics中将Marketo生成的营销列表与Campaign分离。

## 从Dynamics营销活动中移除 {#remove-from-dynamics-campaign}

此流程步骤可以在Marketo Smart Campaigns中使用，以从Microsoft营销活动中移除人员。 这只会从营销活动中删除那些之前通过“添加到Microsoft Campaign”的流量操作添加到营销活动中的潜在客户。

>[!NOTE]
>
>此流程操作仅适用于触发营销活动。

在智能营销策划中，查找并选择要从中删除人员的Dynamics营销策划。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果在营销活动列表中未看到Dynamics营销活动：
>
>* 确保Campaign同步正常运行
>* 该营销活动在Microsoft Dynamics中处于非活动状态
