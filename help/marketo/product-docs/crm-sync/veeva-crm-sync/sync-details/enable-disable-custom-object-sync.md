---
description: 启用/禁用自定义对象同步 — Marketo文档 — 产品文档
title: 启用/禁用自定义对象同步
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 启用/禁用自定义对象同步 {#enable-disable-custom-object-sync}

在Veeva CRM实例中创建的自定义对象也可以包含在Marketo Engage中。 下面是如何设置它。

## 启用或禁用自定义对象同步 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**需要管理员权限**

1. 在Marketo中，单击 **管理员**，则 **Veeva对象同步**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. 如果这是您的第一个自定义对象，请单击同步架构。 如果没有，请单击 **刷新架构** 以确保您拥有最新版本。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. 如果全局同步正在运行，请通过单击 **禁用全局同步**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >同步Veeva自定义对象模式可能需要几分钟。

1. 单击 **刷新架构**.

   ![](assets/enable-disable-custom-object-sync-4.png)

选择要同步的对象，然后单击“启用同步”。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo只有与Veeva CRM中的“联系人”或“帐户”对象有直接关系时，才能同步自定义对象。

1. 单击 **启用同步** 再次。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 返回至Veeva选项卡，然后单击 **启用同步**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## 使用自定义对象 {#using-your-custom-objects}

>[!NOTE]
>
>不能在具有触发器的智能营销活动中使用自定义对象。

1. 在您的Smart List中，将拖动到“Has Opportunity”筛选器上，并将设置为 **True**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. （可选）使用过滤器约束来缩小焦点范围。

   ![](assets/enable-disable-custom-object-sync-9.png)

太棒了！ 现在，您可以在智能营销活动和智能列表中使用此自定义对象的数据。

>[!MORELIKETHIS]
>
>[将自定义对象字段添加/删除为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}
