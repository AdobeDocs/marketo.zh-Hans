---
unique-page-id: 2953384
description: 为自定义实体启用同步 — Marketo文档 — 产品文档
title: 为自定义实体启用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# 为自定义实体启用同步 {#enable-sync-for-a-custom-entity}

如果您需要来自Dynamics的自定义实体数据才能在Marketo中使用，以下是如何为其启用同步的。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>* 为自定义实体启用同步后，Marketo会执行初始同步，以引入自定义对象的所有数据。
>* 营销列表和营销列表成员包括 **不支持** 此时。

>[!IMPORTANT]
>
>Marketo同步用户需要具有自定义对象的读取权限才能列出该自定义对象并对其执行同步。

1. 转到 **管理员** 部分。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 选择 **Microsoft Dynamics** 并单击 **禁用同步**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >要启用或禁用自定义实体，必须暂时禁用全局同步。

1. 在数据库管理下，单击 **Dynamics实体同步** 链接。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 单击 **同步架构** 链接。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 选择要同步的实体，然后单击 **启用同步**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 选择要同步或用作的字段 [约束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和/或触发智能列表。 完成后，单击 **启用同步**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >在同步过程中，您可能会注意到“动态实体同步”项目从导航树中消失。 这是预期行为，同步完成后它将重新显示。

1. 现在，实体上有一个绿色复选标记。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. 不要忘记重新启用全局同步！

   ![](assets/enable-sync-for-a-custom-entity-8.png)
