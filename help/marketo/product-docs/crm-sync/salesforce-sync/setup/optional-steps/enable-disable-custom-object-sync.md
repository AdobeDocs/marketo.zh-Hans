---
unique-page-id: 4719297
description: 启用/禁用自定义对象同步 — Marketo文档 — 产品文档
title: 启用/禁用自定义对象同步
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 启用/禁用自定义对象同步 {#enable-disable-custom-object-sync}

在Salesforce实例中创建的自定义对象也可以是Marketo Engage的一部分。 下面是设置方法。

## 启用/禁用自定义对象同步 {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**需要管理员权限**

1. 单击&#x200B;**[!UICONTROL 管理员]**。

   ![](assets/one.png)

1. 在“数据库管理”菜单中，单击&#x200B;**[!UICONTROL Salesforce对象同步]**。

   ![](assets/two-2.png)

1. 如果这是您的第一个自定义对象，请单击&#x200B;**[!UICONTROL 同步架构]**。 否则，请单击&#x200B;**[!UICONTROL 刷新架构]**&#x200B;以确保您拥有最新的架构。

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. 如果全局同步正在运行，则必须通过单击&#x200B;**[!UICONTROL 禁用全局同步]**&#x200B;来禁用它。

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >同步Salesforce自定义对象架构可能需要几分钟时间。

1. 单击&#x200B;**[!UICONTROL 刷新架构]**。

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. 选择要同步的对象，然后单击&#x200B;**[!UICONTROL 启用同步]**。

   >[!TIP]
   >
   >Marketo只能同步自定义对象，前提是它与Salesforce中的Lead、Contact或Account对象存在直接关系。

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. 再次单击&#x200B;**[!UICONTROL 启用同步]**。

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. 返回&#x200B;**[!DNL Salesforce]**&#x200B;选项卡并单击&#x200B;**[!UICONTROL 启用同步]**。

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## 使用自定义对象 {#using-your-custom-objects}

>[!NOTE]
>
>不能将智能营销活动中的自定义对象与触发器一起使用。

1. 在智能列表中，拖到&#x200B;**[!UICONTROL Has Opportunity]**&#x200B;筛选器上并设置为&#x200B;**[!UICONTROL true]**。

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. 然后，使用筛选约束缩小焦点。

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   太棒了！ 现在，您可以在智能营销活动和智能列表中使用此自定义对象的数据。

>[!MORELIKETHIS]
>
>[添加/删除自定义对象字段作为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
