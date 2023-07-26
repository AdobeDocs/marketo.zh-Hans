---
unique-page-id: 10099680
description: 导入自定义对象数据 — Marketo文档 — 产品文档
title: 导入自定义对象数据
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 导入自定义对象数据 {#import-custom-object-data}

可以轻松地将自定义对象数据导入数据库。 如果对公司使用自定义对象，请参阅 [在公司中使用自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) 以了解更多信息。

1. 在“我的Marketo”中，转到 **[!UICONTROL 数据库]**.

   ![](assets/import-custom-object-data-1.png)

1. 单击 **[!UICONTROL 新建]** 并选择 **[!UICONTROL 导入自定义对象数据]**.

   ![](assets/import-custom-object-data-2.png)

1. 单击 **[!UICONTROL 浏览]** 以查找数据文件。 选择文件格式（在此示例中为逗号分隔值）。

   ![](assets/import-custom-object-data-3.png)

1. 选择您的 [!UICONTROL 自定义对象].

   ![](assets/import-custom-object-data-4.png)

1. 选择 [!UICONTROL 重复数据删除模式] 从下拉菜单中查找。 单击 **[!UICONTROL 下一个]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >在创建或更新自定义对象记录时，使用重复数据删除字段作为唯一标识符。 此示例使用的“重复数据删除”字段 **car** 自定义对象 — vin（车辆ID号）。 如果仅更新自定义对象记录，则可以选择 [!UICONTROL Marketo Guid] 作为 [!UICONTROL 重复数据删除模式].

1. 将每列映射到Marketo字段，然后从下拉列表中选择该字段。

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >确保文件中的值与您匹配的字段类型（例如，文本、整数等）匹配，否则文件将被拒绝。

1. 单击 **[!UICONTROL 下一个]**.

   ![](assets/import-custom-object-data-7.png)

1. 单击 **[!UICONTROL 导入]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >自定义对象的大小限制为100MB。

   >[!TIP]
   >
   >在“ ”中输入您的电子邮件地址 **[!UICONTROL 发送警报到]** 字段和Marketo将在导入完成后通过电子邮件发送给您！

1. 在屏幕右上角，您将在导入运行时看到通知，并在导入完成后看到最终结果。

   ![](assets/import-custom-object-data-9.png)

   好耶！

>[!MORELIKETHIS]
>
>[了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
