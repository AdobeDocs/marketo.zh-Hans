---
unique-page-id: 12983101
description: 将自定义字段映射到Marketo - Marketo文档 — 产品文档
title: 将自定义字段映射到 Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 5%

---

# 将自定义字段映射到 Marketo {#map-custom-fields-to-marketo}

默认情况下，您可能希望收集到的信息比[!DNL Facebook]存储的标准信息多，例如某人使用您的在线交付服务的频率。 您可以通过在[潜在客户广告中](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink)创建自定义问题[!DNL Facebook]来完成此操作。

但是，**Marketo不会自动开始收集此数据**。 为了让Marketo开始捕获自定义字段值，您&#x200B;**必须**&#x200B;将这些自定义字段映射到Marketo中的字段。

以下是在“管理”的LaunchPoint区域中设置此步骤的方法。

>[!NOTE]
>
>**需要管理员权限**

1. 转到“管理”区域并单击&#x200B;**[!UICONTROL LaunchPoint]**。 在“已安装的服务”下，查找并编辑&#x200B;**[!UICONTROL Facebook Lead Ads]**。

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. 将授权帐户保持原样 — 请&#x200B;**不**&#x200B;进行任何更改。 单击 **[!UICONTROL Next]**。

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. 与以前一样，将所选页面保持不变 — 请&#x200B;**不**&#x200B;进行任何更改。 单击 **[!UICONTROL Next]**。

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. 在这里，您可以将自定义[!DNL Facebook]字段映射到您的Marketo字段。 单击&#x200B;**[!UICONTROL Add].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. 在新行中，输入[!DNL Facebook]自定义字段的名称。

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >只有已保存到[!DNL Facebook]表单模板的字段才会在此处显示为选项。

1. 在&#x200B;**[!UICONTROL Marketo Field]**&#x200B;列中单击。 键入以搜索要映射到的字段。 选择字段后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >如果您在Marketo中尚没有可将[!DNL Facebook]字段映射到其中的字段，了解如何[创建自定义字段](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)。

>[!CAUTION]
>
>您&#x200B;**必须**&#x200B;对所有新[!DNL Facebook]字段执行此过程，以便Marketo收集数据。
