---
description: 在Dynamics Campaign - Marketo文档 — 产品文档中添加或删除人员
title: 在Dynamics Campaign中添加或删除人员
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 在Dynamics Campaign中添加或删除人员 {#add-or-remove-people-from-your-dynamics-campaign}

## 添加到Dynamics Campaign {#add-to-dynamics-campaign}

此流程步骤可在Marketo智能营销活动中使用，在Microsoft营销活动中将人员添加为潜在客户或联系人。 如果Dynamics中尚不存在该潜在客户，则会自动同步该潜在客户并将其添加到营销活动。

>[!NOTE]
>
>此流程操作仅适用于触发器促销活动。

在您的智能营销活动中，查找并选择要将您的人员添加到的Dynamics营销活动。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果在营销活动列表中看不到Dynamics营销活动：
>
>* 确保营销活动同步正常运行
>* 该营销活动在Microsoft Dynamics中不活动


系统会自动创建一个特定于促销活动的静态营销列表，每个列表针对潜在客户和联系人，以将人员添加到其中。 这是一次性操作，在后续同步到营销活动时，会使用相同的营销列表。 静态营销列表名称采用的命名标准是 `Mkto-leads-<uniqueID>` 对于潜在客户和 `Mkto-contacts-<uniqueID>` 联系人。

将这些Marketo生成的营销列表关联到其他营销活动可能会导致行为混乱。 例如：添加到一个营销活动也会导致添加到第二个营销活动。 同样，也不建议在Dynamics中将Marketo生成的营销列表与促销活动分离。

## 从Dynamics Campaign中删除 {#remove-from-dynamics-campaign}

此流程步骤可在Marketo智能营销活动中使用，从Microsoft营销活动中删除人员。 这会仅删除之前通过“已添加到Microsoft促销活动”流程操作添加到促销活动的促销活动中的那些潜在客户。

>[!NOTE]
>
>此流程操作仅适用于触发器促销活动。

在您的智能营销活动中，找到并选择要从中删除人员的Dynamics营销活动。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果您在营销活动列表中未看到Dynamics营销活动：
>
>* 确保营销活动同步正常运行
>* 该营销活动在Microsoft Dynamics中不活动

