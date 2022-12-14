---
unique-page-id: 2953384
description: 为自定义实体启用同步 — Marketo文档 — 产品文档
title: 为自定义实体启用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: 79cfb0396f690a370cdce4e4df3a23c7439c252e
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# 为自定义实体启用同步 {#enable-sync-for-a-custom-entity}

如果您需要Dynamics中的自定义实体数据才能在Marketo中使用，请参阅下面介绍如何为其启用同步。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>* 为自定义实体启用同步时，Marketo会执行初始同步以引入自定义对象的所有数据。
>* 营销列表和营销列表成员包括 **不受支持** 此时。


>[!IMPORTANT]
>
>Marketo同步用户需要对自定义对象的读取访问权限才能列出该对象并对其执行同步。

1. 转到 **管理员** 中。

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. 选择 **Microsoft Dynamics** 单击 **禁用同步**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >必须临时禁用全局同步才能启用或禁用自定义实体。

1. 在“数据库管理”下，单击 **Dynamics实体同步** 链接。

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. 单击 **同步模式** 链接。

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. 选择要同步的实体并单击 **启用同步**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. 选择要同步或用作的字段 [约束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) 和/或触发器。 完成后，单击 **启用同步**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >在同步过程中，您可能会注意到“动态实体同步”项目从导航树中消失。 这是预期行为，它将在同步完成后重新显示。

1. 该实体现在具有绿色复选标记。

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. 不要忘记重新启用全局同步！

   ![](assets/enable-sync-for-a-custom-entity-8.png)
