---
description: 了解如何将Dynamic Chat连接到您的Marketo Engage订阅。 执行一次性同步并选择要定位的人员和公司属性。
title: Adobe Marketo Engage
feature: Dynamic Chat
exl-id: 9ce43de3-0503-4894-89f2-ee24e7df9a73
TQID: https://experienceleague.adobe.com/n8HC8kkHZguZoZ2eBijiUetTrX1rY0ZLN0lIhZGUUcg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: cc2b43cd0e963803d1998bd8438f066d74303e67
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 3%

---

# Adobe Marketo Engage {#adobe-marketo-engage}

## 连接Dynamic Chat {#connecting-dynamic-chat}

完成[初始设置](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md){target="_blank"}后，便可以执行一次性同步，将Dynamic Chat连接到Adobe Marketo Engage订阅。

>[!NOTE]
>
>Dynamic Chat支持同步[Marketo native](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/field-types){target="_blank"}以及自定义人员字段和公司字段。

1. 在“我的Marketo”中，单击&#x200B;**[!UICONTROL Dynamic Chat]**&#x200B;磁贴。

   ![](assets/adobe-marketo-engage-1.png)

   >[!NOTE]
   >
   >如果您在“我的Marketo”屏幕中未看到Dynamic Chat磁贴，请从experience.adobe.com上的“应用程序”菜单访问Dynamic Chat，并通过&#x200B;**配置** > **集成**&#x200B;连接到Marketo。 连接后，将显示拼贴。

1. 如果您之前曾使用Adobe ID访问过应用程序，则会直接转到Dynamic Chat。 如果没有，[请设置您的Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html){target="_blank"}。

1. 要连接您的Marketo实例，请选择&#x200B;**[!UICONTROL Integrations]**。

   ![](assets/adobe-marketo-engage-2.png)

1. 在Marketo信息卡上，单击&#x200B;**[!UICONTROL Initiate Sync]**。

   ![](assets/adobe-marketo-engage-3.png)

1. 从您的Marketo实例中选择最多50个属性（标准或自定义字段）以同步到Dynamic Chat，用于受众定位、数据映射和个性化。 完成后，单击 **[!UICONTROL Next]**。

   ![](assets/adobe-marketo-engage-4.png)

1. 查看您的选择。 单击&#x200B;**[!UICONTROL Confirm]**&#x200B;启动同步。

   ![](assets/adobe-marketo-engage-5.png)

>[!NOTE]
>
>同步可能需要2到24小时才能完成，具体取决于数据库的大小。

## 添加属性 {#add-an-attribute}

初次同步后，请按照以下步骤添加其他属性。

1. 在&#x200B;**[!UICONTROL Integrations]**&#x200B;中，验证是否已选择&#x200B;**[!UICONTROL Adobe Marketo Engage]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL Add Attribute]**。

   ![](assets/adobe-marketo-engage-6.png)

1. 选择要添加的属性，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/adobe-marketo-engage-7.png)

1. 查看您的选择，然后单击&#x200B;**[!UICONTROL Confirm]**。

   ![](assets/adobe-marketo-engage-8.png)

## 删除属性 {#remove-an-attribute}

初次同步后，请按照以下步骤删除属性。

>[!NOTE]
>
>只有属性当前未被任何对话框使用时，您才会看到用于移除该属性的选项。

1. 在&#x200B;**[!UICONTROL Integrations]**&#x200B;中，验证是否已选择&#x200B;**[!UICONTROL Adobe Marketo Engage]**&#x200B;选项卡，然后单击要删除的属性。

   ![](assets/adobe-marketo-engage-9.png)

1. 单击 **[!UICONTROL Remove Attribute]**。

   ![](assets/adobe-marketo-engage-10.png)

>[!MORELIKETHIS]
>
>[初始设置](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md){target="_blank"}
