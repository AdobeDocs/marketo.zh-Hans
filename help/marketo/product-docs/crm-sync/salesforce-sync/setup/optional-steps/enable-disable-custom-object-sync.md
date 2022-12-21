---
unique-page-id: 4719297
description: 启用/禁用自定义对象同步 — Marketo文档 — 产品文档
title: 启用/禁用自定义对象同步
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 启用/禁用自定义对象同步 {#enable-disable-custom-object-sync}

在Salesforce实例中创建的自定义对象也可以包含在Marketo中。 下面是如何设置它。

## 启用/禁用自定义对象同步 {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>需要管理员权限。

1. 单击 **管理员**.

   ![](assets/one.png)

1. 在“数据库管理”菜单中，单击 **Salesforce对象同步**.

   ![](assets/two-2.png)

1. 如果这是您的第一个自定义对象，请单击 **同步架构。** 否则，请单击 **刷新架构** 以确保您拥有最新版本。

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. 如果全局同步正在运行，则必须通过单击 **禁用全局同步。**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >同步Salesforce自定义对象架构可能需要几分钟时间。

1. 单击 **刷新架构**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 选择要同步的对象并单击 **启用同步**.

   >[!TIP]
   >
   >Marketo只有与Salesforce中的Lead、Contact或Account对象有直接关系时，才能同步自定义对象。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 单击 **启用同步** 再次。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 返回到 **Salesforce** 选项卡，单击 **启用同步**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## 使用自定义对象 {#using-your-custom-objects}

>[!NOTE]
>
>不能在具有触发器的智能营销活动中使用自定义对象。

1. 在智能列表中，将 **有机会** 筛选器和设置为 **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 然后，使用过滤器约束来缩小焦点范围。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   太棒了！ 现在，您可以在智能营销活动和智能列表中使用此自定义对象的数据。

>[!MORELIKETHIS]
>
>[将自定义对象字段添加/删除为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
