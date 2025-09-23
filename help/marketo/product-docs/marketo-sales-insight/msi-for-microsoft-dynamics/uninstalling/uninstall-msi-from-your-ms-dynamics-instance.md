---
unique-page-id: 37355600
description: 从MS [!DNL Dynamics] 实例中卸载MSI - Marketo文档 — 产品文档
title: 从MS [!DNL Dynamics] 实例卸载MSI
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 3%

---

# 从MS [!DNL Dynamics]实例卸载MSI {#uninstall-msi-from-your-ms-dynamics-instance}

若要从MS [!DNL Dynamics]实例卸载MSI，您需要同时在Marketo和MS [!DNL Dynamics]中执行步骤。

>[!PREREQUISITES]
>
>[禁用全局MS [!DNL Dynamics] 同步](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/one-1.png)

1. 单击 **[!UICONTROL Sales Insight]**。

   ![](assets/six.png)

1. 单击 **[!UICONTROL Edit Field Sync]**。

   ![](assets/seven.png)

1. 选中&#x200B;**[!UICONTROL Disable Sync]**&#x200B;复选框并单击&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >确保在禁用字段同步之前[禁用全局MS Dynamics同步](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)。

   ![](assets/eight.png)

## 在MS [!DNL Dynamics]实例中执行以下步骤： {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 单击 **[!UICONTROL Advanced Settings]**。

1. 单击 **[!UICONTROL Solutions]**。

1. 选择&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;并单击删除图标。

1. 当出现Uninstall Solution模式时，单击&#x200B;**[!UICONTROL OK]**。

   完全卸载MS [!DNL Dynamics]解决方案通常需要大约20分钟。 但是，如果您有一个大的MS [!DNL Dynamics]实例，则可能需要更长的时间。

   >[!NOTE]
   >
   >卸载MSI后，请记得打开全局MS [!DNL Dynamics]同步。
