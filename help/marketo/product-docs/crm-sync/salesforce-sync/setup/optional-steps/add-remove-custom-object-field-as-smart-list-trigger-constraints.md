---
unique-page-id: 4719300
description: 添加/删除自定义对象字段作为智能列表/触发器约束 — Marketo文档 — 产品文档
title: 添加/删除自定义对象字段作为智能列表/触发器约束
exl-id: 639e73eb-9a8c-4b10-8e97-892abf5c5db0
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 1%

---

# 添加/删除自定义对象字段作为智能列表/触发器约束 {#add-remove-custom-object-field-as-smart-list-trigger-constraints}

Marketo Engage提供了对Salesforce自定义对象同步的细粒度控制。 这允许您选择可用作自定义对象过滤器中的约束条件的字段，并在智能营销策划中将其用作触发器。

>[!NOTE]
>
>**需要管理员权限**

1. 已转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域。

   ![](assets/add-remove-custom-object-field-1.png)

1. 单击 **[!UICONTROL Salesforce Objects Sync]**。

   ![](assets/image2015-12-11-15-3a11-3a41.png)

1. **[!UICONTROL Salesforce Objects Sync]**&#x200B;显示在左列。

   ![](assets/image2015-12-11-15-3a15-3a15.png)

1. 选择要修改的对象。

   ![](assets/image2014-12-10-13-3a10-3a11.png)

1. 单击 **[!UICONTROL Edit Visible Fields]**。

   >[!TIP]
   >
   >如果&#x200B;**[!UICONTROL Edit Visible Fields]**&#x200B;按钮呈灰显状态，则该对象当前正用于智能列表或智能营销活动中。 删除所有关联以继续。

   ![](assets/image2014-12-10-13-3a10-3a25.png)

1. 如果已启用全局同步，请单击&#x200B;**[!UICONTROL Disable Global Sync]**。

   ![](assets/image2014-12-10-13-3a10-3a36.png)

1. 选中所需的筛选器/触发器约束旁边的框，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-10-13-3a10-3a47.png)

   >[!NOTE]
   >
   >默认情况下，选择所有字段作为筛选条件的限制。

1. 单击&#x200B;**[!UICONTROL Fields]**&#x200B;选项卡以确认更改。

   ![](assets/image2014-12-10-13-3a10-3a56.png)

   >[!NOTE]
   >
   >不要忘记重新启用全局同步！

现在，您的智能列表和智能营销活动具有更强的功能。

>[!MORELIKETHIS]
>
>[启用/禁用自定义对象同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-custom-object-sync.md){target="_blank"}
