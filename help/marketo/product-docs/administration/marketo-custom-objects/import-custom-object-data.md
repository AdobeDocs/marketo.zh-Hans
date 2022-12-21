---
unique-page-id: 10099680
description: 导入自定义对象数据 — Marketo文档 — 产品文档
title: 导入自定义对象数据
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 导入自定义对象数据 {#import-custom-object-data}

将自定义对象数据导入数据库很容易。 如果您正在公司中使用自定义对象，请参阅 [在公司中使用自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) 以了解更多信息。

1. 在我的Marketo中，转到 **数据库**.

   ![](assets/db-1.png)

1. 单击 **新建** 选择 **导入自定义对象数据**.

   ![](assets/image2016-4-7-10-6-54.png)

1. 单击 **浏览** 来查找数据文件。 选择文件格式（此示例中的逗号分隔值）。

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. 选择您的自定义对象。

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. 从下拉列表中选择重复数据消除模式。 单击 **下一个**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >在创建或更新自定义对象记录时，使用重复数据删除字段作为唯一标识符。 此示例使用 **汽车** 自定义对象 — vin（车辆ID号）。 如果只更新自定义对象记录，则可以选择Marketo Guid作为重复数据消除模式。

1. 将每列映射到一个Marketo字段，然后从下拉列表中选择该字段。

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >确保文件中的值与您要匹配的字段类型（例如，文本、整数等）匹配，否则将拒绝文件。

1. 单击 **下一个**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. 单击 **导入**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >自定义对象的大小限制为100MB。

   >[!TIP]
   >
   >在 **将警报发送到：** 字段，Marketo会在导入完成后向您发送电子邮件！

1. 在屏幕的右上角，您将在导入运行时看到通知，并在完成时看到最终结果。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   耶！

>[!MORELIKETHIS]
>
>[了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
