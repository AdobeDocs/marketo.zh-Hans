---
description: 从您的Dynamics活动添加或删除人物 — Marketo文档 — 产品文档
title: 从Dynamics活动添加或删除人物
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 从Dynamics活动{#add-or-remove-people-from-your-dynamics-campaign}添加或删除人物

## 添加到Dynamics活动{#add-to-dynamics-campaign}

此流程步骤可用于Marketo智能活动，以在Microsoft活动中将人员添加为潜在客户或联系人。 如果Dynamics中尚不存在该潜在客户，则它将自动同步到该活动并添加到该潜在客户。

>[!NOTE]
>
>此流动操作仅适用于触发活动。

在智能活动中，查找并选择要将人员添加到的Dynamics活动。

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>如果在活动列表中看不到Dynamics活动:
>
>* 确保活动同步正常工作
>* 活动在Microsoft Dynamics中不活动


系统会自动创建一个特定于活动的静态营销列表，每个营销分别用于潜在客户和联系人，以将人员添加到其中。 这是一次性操作，只需对活动进行一次后续同步，即可使用同一营销列表。 静态营销列表名称采用的命名标准是`Mkto-leads-<uniqueID>`（对于潜在客户）和`Mkto-contacts-<uniqueID>`（对于联系人）。

将这些Marketo生成的营销列表关联到其他活动可能会导致行为混乱。 例如：添加到一个活动也会导致添加到第二个活动。 同样，也不建议将Marketo生成的营销列表与Dynamics中的活动分离。

## 从Dynamics活动{#remove-from-dynamics-campaign}中删除

此流程步骤可用于Marketo智能活动，以从Microsoft活动中删除人员。 这将仅删除之前通过“添加到Microsoft活动”流动操作添加到活动中的那些Lead。

>[!NOTE]
>
>此流动操作仅适用于触发活动。

在智能活动中，找到并选择要从中删除您的人员的Dynamics活动。

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>如果您在活动列表中未看到Dynamics活动:
>
>* 确保活动同步正常工作
>* 活动在Microsoft Dynamics中不活动

