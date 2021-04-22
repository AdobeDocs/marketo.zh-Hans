---
unique-page-id: 4719300
description: 添加/删除自定义对象字段作为智能列表/触发器约束 — Marketo文档 — 产品文档
title: 添加/删除自定义对象字段作为智能列表/触发器约束
exl-id: 639e73eb-9a8c-4b10-8e97-892abf5c5db0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 添加/删除自定义对象字段作为智能列表/触发器约束{#add-remove-custom-object-field-as-smart-list-trigger-constraints}

Marketo提供对Salesforce自定义对象同步的精细控制。 这允许您选择自定义对象过滤器中可用作约束的字段，并在智能活动中将这些字段用作触发器。

>[!NOTE]
>
>**需要管理权限**

1. 单击&#x200B;**管理。**

   ![](assets/image2014-12-10-13-3a9-3a47.png)

1. 单击&#x200B;**Admin**，然后单击&#x200B;**Salesforce对象同步。**

   ![](assets/image2015-12-11-15-3a11-3a41.png)

1. **Salesforce对象** 在左列中同步。

   ![](assets/image2015-12-11-15-3a15-3a15.png)

1. 选择要修改的对象。

   ![](assets/image2014-12-10-13-3a10-3a11.png)

1. 单击&#x200B;**编辑可见字段**。

   >[!TIP]
   >
   >如果&#x200B;**“编辑可见字段”**&#x200B;按钮灰显，则该对象当前正在智能列表或智能活动中使用。 删除所有关联以继续。

   ![](assets/image2014-12-10-13-3a10-3a25.png)

1. 如果已启用全局同步，请单击&#x200B;**禁用全局同步**。

   ![](assets/image2014-12-10-13-3a10-3a36.png)

1. 选中所需的过滤器/触发器约束旁边的框，然后单击&#x200B;**保存**。

   ![](assets/image2014-12-10-13-3a10-3a47.png)

   >[!NOTE]
   >
   >默认情况下，所有字段都处于选中状态，以成为过滤器的约束。

1. 单击&#x200B;**字段**&#x200B;选项卡以确认更改。

   ![](assets/image2014-12-10-13-3a10-3a56.png)

   >[!NOTE]
   >
   >不要忘记重新启用全局同步！

哇！ 现在，您的智能列表和智能活动的强大功能已更强大。

>[!MORELIKETHIS]
>
>[启用/禁用自定义对象同步](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-custom-object-sync.md)
