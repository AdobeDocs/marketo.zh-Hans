---
unique-page-id: 2953384
description: 为自定义实体启用同步 — Marketo Docs — 产品文档
title: 为自定义实体启用同步
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 为自定义实体{#enable-sync-for-a-custom-entity}启用同步

如果您需要Dynamics中的自定义实体数据才能在Marketo中使用，下面将介绍如何为其启用同步：

>[!NOTE]
>
>**需要管理权限**

1. 转至&#x200B;**Admin**&#x200B;部分。

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. 选择&#x200B;**Microsoft Dynamics**&#x200B;并单击&#x200B;**禁用同步**。

   必须临时禁用全局同步才能启用或禁用自定义实体。

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. 在“数据库管理”下，单击&#x200B;**Dynamics Entities Sync**&#x200B;链接。

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. 单击&#x200B;**同步模式**&#x200B;链接。

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. 选择要同步的实体，然后单击&#x200B;**启用同步**。

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. 选择要同步的字段，或在智能列表中用作[约束](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)和/或触发器。 完成后，单击&#x200B;**启用同步**。

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >在同步过程中，您可能会注意到“动态实体同步”项从导航树中消失。 这是预期行为，同步完成后将重新显示。

1. 实体现在具有绿色复选标记。

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. 别忘了重新启用全局同步！

   ![](assets/image2015-11-10-9-3a48-3a35.png)

哦耶！ 强大的功能。
