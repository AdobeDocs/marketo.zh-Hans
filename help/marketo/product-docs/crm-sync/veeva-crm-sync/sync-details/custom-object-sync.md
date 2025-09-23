---
description: 自定义对象同步 — Marketo文档 — 产品文档
title: 自定义对象同步
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 5%

---

# 自定义对象同步 {#custom-object-sync}

在[!DNL Veeva] CRM实例中创建的自定义对象也可以是Marketo Engage的一部分。 下面是设置方法。

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>要使用自定义对象，必须将其关联到[!DNL Veeva] CRM中的联系人或帐户对象。

## 启用自定义对象 {#enable-custom-object}

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**，然后单击&#x200B;**[!UICONTROL Veeva Objects Sync]**。

   ![](assets/custom-object-sync-1.png)

1. 如果这是您的第一个自定义对象，请单击&#x200B;**[!UICONTROL Sync Schema]**。

   ![](assets/custom-object-sync-2.png)

1. 单击 **[!UICONTROL Disable Global Sync]**。

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >[!DNL Veeva]自定义对象架构的初始同步可能需要几分钟时间。

1. 将要同步的自定义对象拖到画布中。

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >自定义对象必须具有唯一的名称。 Marketo不支持具有相同名称的两个其他自定义对象。

1. 单击 **[!UICONTROL Enable Sync]**。

   ![](assets/custom-object-sync-5.png)

1. 再次单击&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/custom-object-sync-6.png)

1. 返回&#x200B;**[!UICONTROL Veeva]**&#x200B;选项卡。

   ![](assets/custom-object-sync-7.png)

1. 单击 **[!UICONTROL Enable Sync]**。

   ![](assets/custom-object-sync-8.png)

1. 要查看您的所有[!DNL Veeva]自定义对象，请单击&#x200B;**[!UICONTROL Admin]**&#x200B;和&#x200B;**[!UICONTROL Veeva Objects Sync]**。

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo仅支持链接到一到两层深标准实体的自定义实体。

太棒了！ 现在，您可以在智能营销活动和智能列表中使用此自定义对象中的数据。

>[!MORELIKETHIS]
>
>* [正在同步呼叫和呼叫关键消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [添加/删除自定义对象字段作为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
