---
unique-page-id: 10094188
description: 批准自定义对象 — Marketo文档 — 产品文档
title: 批准自定义对象
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 批准自定义对象 {#approve-a-custom-object}

您必须先批准自定义对象，然后才能使用它。 对于新自定义对象和您编辑的自定义对象，此过程略有不同。

## 批准新的自定义对象 {#approve-a-new-custom-object}

您已创建一个全新的自定义对象。 下面是如何批准它的。

1. 转到&#x200B;**[!UICONTROL 管理员]**&#x200B;区域。

   ![](assets/approve-a-custom-object-1.png)

1. 单击&#x200B;**[!UICONTROL Marketo自定义对象]**。

   ![](assets/approve-a-custom-object-2.png)

1. 选择处于“草稿”状态的对象。

   ![](assets/approve-a-custom-object-3.png)

1. 单击&#x200B;**[!UICONTROL 自定义对象操作]**&#x200B;下拉列表，然后选择&#x200B;**[!UICONTROL 批准对象]**。

   ![](assets/approve-a-custom-object-4.png)

1. 状态更改为[!UICONTROL 已批准]。

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >在&#x200B;_一对多结构_&#x200B;中使用的自定义对象必须具有至少一个要批准的重复数据删除字段、链接字段、链接对象名称和链接字段名称。
   >
   >在&#x200B;_多对多结构_ **中使用的自定义对象在批准时不需要链接字段、链接对象名称或链接字段名称（因为它们位于中间对象中）。**
   >
   >用作&#x200B;_中间对象_&#x200B;的自定义对象需要链接字段、链接对象名称和链接字段名称，但&#x200B;**不**&#x200B;需要重复数据删除字段。
   >
   >有关详细信息，请参阅[了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)。

就是这样！ 现在，您可以在筛选器和触发器的限制中选择自定义对象以在营销活动中使用。

## 批准已编辑的自定义对象 {#approve-an-edited-custom-object}

编辑已批准的自定义对象后，必须批准草稿才能将自定义对象恢复到“已批准”状态。

1. 编辑已批准的自定义对象时，它将收到[!UICONTROL 已批准草稿]状态。

   ![](assets/approve-a-custom-object-6.png)

1. 准备好批准草稿后，单击&#x200B;**[!UICONTROL 自定义对象操作]**&#x200B;下拉列表，然后选择&#x200B;**[!UICONTROL 批准对象]**。

   ![](assets/approve-a-custom-object-7.png)

1. 预览显示草稿中更改的项目。 单击&#x200B;**[!UICONTROL 批准]**。

   ![](assets/approve-a-custom-object-8.png)
