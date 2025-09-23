---
description: 启用/禁用自定义对象同步 — Marketo文档 — 产品文档
title: 启用/禁用自定义对象同步
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 5%

---

# 启用/禁用自定义对象同步 {#enable-disable-custom-object-sync}

在[!DNL Veeva] CRM实例中创建的自定义对象也可以是Marketo Engage的一部分。 下面是设置方法。

## 启用或禁用自定义对象同步 {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**需要管理员权限**

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**，然后单击&#x200B;**[!UICONTROL Veeva Objects Sync]**。

   ![](assets/enable-disable-custom-object-sync-1.png)

1. 如果这是您的第一个自定义对象，请单击&#x200B;**[!UICONTROL Sync Schema]**。 如果没有，请单击&#x200B;**[!UICONTROL Refresh Schema]**&#x200B;以确保您拥有最新版本。

   ![](assets/enable-disable-custom-object-sync-2.png)

1. 如果全局同步正在运行，请单击&#x200B;**[!UICONTROL Disable Global Sync]**&#x200B;将其禁用。

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >同步[!DNL Veeva]自定义对象架构可能需要几分钟时间。

1. 单击 **[!UICONTROL Refresh Schema]**。

   ![](assets/enable-disable-custom-object-sync-4.png)

选择要同步的对象，然后单击&#x200B;**[!UICONTROL Enable Sync]**。

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo只能同步自定义对象，前提是它与[!DNL Veeva] CRM中的联系人或帐户对象存在直接关系。

1. 再次单击&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/enable-disable-custom-object-sync-6.png)

1. 返回[!UICONTROL Veeva]选项卡并单击&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/enable-disable-custom-object-sync-7.png)

## 使用自定义对象 {#using-your-custom-objects}

>[!NOTE]
>
>您不能在带有触发器的智能营销活动中使用自定义对象。

1. 在您的[!UICONTROL Smart List]中，拖到&quot;**[!UICONTROL Has Opportunity]**&quot;筛选器上并设置为&#x200B;**[!UICONTROL True]**。

   ![](assets/enable-disable-custom-object-sync-8.png)

1. （可选）使用筛选条件约束来缩小焦点。

   ![](assets/enable-disable-custom-object-sync-9.png)

太棒了！ 您现在可以在[!UICONTROL Smart Campaigns]和[!UICONTROL Smart Lists]中使用此自定义对象的数据。

>[!MORELIKETHIS]
>
>[添加/删除自定义对象字段作为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
