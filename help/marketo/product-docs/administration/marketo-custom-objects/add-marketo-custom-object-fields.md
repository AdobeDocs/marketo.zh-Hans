---
unique-page-id: 10093688
description: 添加Marketo自定义对象字段 — Marketo文档 — 产品文档
title: 添加Marketo自定义对象字段
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
source-git-commit: 4a33b192cc22550c75769b383e261ac0a86e7ddb
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 添加Marketo自定义对象字段 {#add-marketo-custom-object-fields}

创建自定义对象后，您需要向其添加字段以满足业务需求。

字段定义自定义对象使用的特定信息。 链接字段具有连接自定义对象的特殊作业，并且包含在 [单独文章](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/add-marketo-custom-object-fields-1.png)

1. 单击 **[!UICONTROL Marketo自定义对象]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. 选择要在右侧添加字段的对象。

   ![](assets/add-marketo-custom-object-fields-3.png)

1. 单击 **[!UICONTROL 字段]** 选项卡，然后 **[!UICONTROL 新建字段]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >在您创建自定义对象时，Marketo会自动创建以上显示的三个字段。 Marketo会自动管理这些字段，您无法编辑或删除它们。

1. 输入 [!UICONTROL 显示名称] 和（可选） [!UICONTROL 描述].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >API名称只有在获得批准后才能编辑。

1. 现在，选择适当的 [!UICONTROL 数据类型] 从名单上。

   ![](assets/add-marketo-custom-object-fields-6.png)

1. 提取 [!UICONTROL 重复数据删除] 如果要将新字段用作唯一标识符，请滑动。 单击 **[!UICONTROL 保存]** 完成。

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >重复数据消除字段可用于检索、更新或删除自定义对象。 每个自定义对象定义都必须包含至少一个（且不能超过三个）重复数据消除字段。

1. 添加您需要的任何其他字段。

   >[!NOTE]
   >
   >如果要构建一对多结构，则需要将链接字段添加到自定义对象。 对于多对多结构，自定义对象中不需要链接字段，但必须在中间对象中添加两个链接字段。 参见 [添加Marketo自定义对象链接字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) 创建链接字段，以及 [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) 以了解有关自定义对象类型的详细信息。

>[!MORELIKETHIS]
>
>* [添加Marketo自定义对象链接字段](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [编辑和删除Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [编辑和删除Marketo自定义对象字段](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

