---
unique-page-id: 10099680
description: 导入自定义对象数据 — Marketo Docs — 产品文档
title: 导入自定义对象数据
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 导入自定义对象数据{#import-custom-object-data}

将自定义对象数据导入数据库很容易。 如果要使用带公司的自定义对象，请参阅[使用带公司的自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies)以了解详细信息。

1. 在“我的Marketo”中，转至&#x200B;**Database**。

   ![](assets/db-1.png)

1. 单击&#x200B;**新建**&#x200B;并选择&#x200B;**导入自定义对象数据**。

   ![](assets/image2016-4-7-10-6-54.png)

1. 单击&#x200B;**浏览**&#x200B;以找到数据文件。 选择文件格式（此示例中的逗号分隔值）。

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. 选择您的自定义对象。

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. 从下拉菜单中选择重复数据消除模式。 单击&#x200B;**下一步**。

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >在创建或更新自定义对象记录时，使用重复数据消除字段作为唯一标识符。 此示例使用&#x200B;**car**&#x200B;自定义对象 — vin（车辆ID号）的“重复数据消除”字段。 如果只更新自定义对象记录，则可以选择Marketo Guid作为重复数据消除模式。

1. 将每列映射到一个Marketo字段，然后从下拉菜单中选择它。

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >确保文件中的值与要匹配它们的字段类型（例如，文本、整数等）匹配，否则将拒绝文件。

1. 单击&#x200B;**下一步**。

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. 单击&#x200B;**导入**。

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >自定义对象的大小限制为100MB。

   >[!TIP]
   >
   >在&#x200B;**将警报发送到：**&#x200B;字段中输入您的电子邮件地址，Marketo将在导入完成后通过电子邮件向您发送！

1. 在屏幕的右上角，您将在导入运行时看到通知，并在完成时看到最终结果。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   耶！

>[!MORELIKETHIS]
>
>[了解Marketo自定义对象](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
