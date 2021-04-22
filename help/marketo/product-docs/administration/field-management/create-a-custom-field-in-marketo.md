---
unique-page-id: 2360287
description: 在Marketo - Marketo Docs — 产品文档中创建自定义字段
title: 在Marketo中创建自定义字段
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 在Marketo{#create-a-custom-field-in-marketo}中创建自定义字段

如果您需要Marketo中的新自定义字段来存储/捕获数据，下面将介绍如何创建一个。

1. 转至“Admin”（管理员），然后单击“**Field Management**”。

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >如果您希望这些字段与您的CRM保持同步，请在CRM中创建它们，然后将在Marketo中自动创建它们。

1. 单击&#x200B;**新建自定义字段**。

   ![](assets/two.png)

1. 选择字段“类型”。 这将改变它在Marketo中以智能列表和表单呈现的方式。

   >[!TIP]
   >
   >请查看[自定义字段类型词汇表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)。

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. 输入您希望在Marketo中显示的名称。 将自动生成API名称。 您可以调整它，但设置后无法重命名它。 完成后，单击&#x200B;**创建**。

>[!CAUTION]
>
>字段名称不能开始以下字符：**. &amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>SOAP API和其他后端进程使用API名称。

您现在可以在表单、流程步骤和智能列表中使用此自定义字段！
