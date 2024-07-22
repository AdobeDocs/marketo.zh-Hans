---
unique-page-id: 11378713
description: 触发自定义对象更改 — Marketo文档 — 产品文档
title: 触发自定义对象更改
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: acaf2b421ed65f74bedf18b121ce54e30c19c721
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 触发自定义对象更改 {#trigger-off-custom-object-changes}

>[!NOTE]
>
>此功能仅可用：
>
>* 仅用于Marketo自定义对象，而不用于通过本机[!DNL Salesforce]或[!DNL Microsoft Dynamics]集成同步的自定义对象
>* 作为触发器，而不是过滤器
>
>请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)以启用自定义对象更改触发器。

在智能营销活动的智能列表中，您可以在将自定义对象添加到人员或公司时触发流量操作。 您还可以创建一个在自定义对象中使用&#x200B;_change_&#x200B;作为触发器的智能列表。 例如，使用它可在课程名称更新时发送电子邮件。

>[!NOTE]
>
>更改自定义对象记录时，不会创建活动日志条目。

1. 在Marketo Engage中，转到&#x200B;**[!UICONTROL 营销活动]**。

   ![](assets/trigger-off-custom-object-changes-1.png)

1. 创建或打开现有的Smart Campaign，然后选择智能列表。

   ![](assets/trigger-off-custom-object-changes-2.png)

1. 搜索所需的触发器，并将其拖动到画布上。

   ![](assets/trigger-off-custom-object-changes-3.png)

1. 选择[!UICONTROL 触发器属性]。

   ![](assets/trigger-off-custom-object-changes-4.png)

1. （可选）设置约束。

   ![](assets/trigger-off-custom-object-changes-5.png)

1. 你就在那儿。 更改将自动保存。

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
