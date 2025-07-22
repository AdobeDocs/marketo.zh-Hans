---
unique-page-id: 2953471
description: SFDC同步 — 自定义对象同步 — Marketo文档 — 产品文档
title: SFDC同步 — 自定义对象同步
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---

# SFDC同步：自定义对象同步 {#sfdc-sync-custom-object-sync}

在[!DNL Salesforce]实例中创建的自定义对象也可以是Marketo的一部分。  下面是设置方法。

>[!NOTE]
>
>**需要管理员权限**

>[!PREREQUISITES]
>
>若要使用自定义对象，必须将其关联到[中的](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)潜在客户[、](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)联系人[或](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)帐户[!DNL Salesforce]对象。

>[!IMPORTANT]
>
>Marketo同步用户需要具有自定义对象的读取权限才能列出该自定义对象并对其执行同步。

## 启用自定义对象  {#enable-custom-object}

1. 单击&#x200B;**[!UICONTROL Admin]**&#x200B;和&#x200B;**[!UICONTROL Salesforce Objects Sync]**&#x200B;链接。

   ![](assets/image2015-11-19-10-3a28-3a5.png)。

1. 如果这是您的第一个自定义对象，请单击&#x200B;**[!UICONTROL Sync Schema]**。

   ![](assets/rtaimage-2.png)

1. 单击 **[!UICONTROL Disable Global Sync]**。

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >[!DNL Salesforce]自定义对象架构的初始同步可能需要几分钟时间。

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. 将要同步的自定义对象拖到画布中。

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >自定义对象必须具有唯一的名称。 Marketo不支持具有相同名称的两个其他自定义对象。

1. 单击 **[!UICONTROL Enable Sync]**。

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. 再次单击&#x200B;**[!UICONTROL Enable Sync]**。

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >不要忘记重新启用全局同步！

1. 返回&#x200B;**[!UICONTROL Salesforce]**&#x200B;选项卡。

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. 单击 **[!UICONTROL Enable Sync]**。

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. 要查看您的所有[!DNL Salesforce]自定义对象，请单击&#x200B;**[!UICONTROL Admin]**&#x200B;和&#x200B;**[!UICONTROL Salesforce Objects Sync]**&#x200B;链接（与上述步骤1相同）。

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* Marketo仅支持链接到一到两级深度标准实体的自定义实体。
   >
   >* 自定义对象树可以多次显示同一对象，因为它与主要对象之一（例如，潜在客户、联系人或帐户，或通过中间对象间接连接）的直接连接。 在这种情况下，请选择最接近主对象的对象，然后只选择一个对象。 多次选择同一对象可能会妨碍该自定义对象的同步。

### 后续内容： {#whats-next}

[添加/删除自定义对象字段作为智能列表/触发器约束](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

太棒了！ 现在，您可以在智能营销活动和智能列表中使用此自定义对象中的数据。
