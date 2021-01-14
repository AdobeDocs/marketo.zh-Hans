---
unique-page-id: 2360287
description: 在Marketo - Marketo Docs —— 产品文档中创建自定义字段
title: 在Marketo中创建自定义字段
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# 在Marketo {#create-a-custom-field-in-marketo}中创建自定义字段

如果您需要Market中的新自定义字段来存储／捕获数据，下面将介绍如何创建一个。

1. 转至“管理员”并单击“字段管理”**。**

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >如果希望字段与CRM保持同步，请在CRM中创建这些字段，这些字段将自动在Marketo中创建。

1. 单击&#x200B;**新建自定义字段**。

   ![](assets/two.png)

1. 选择字段类型。 这将改变它在Marketo中以智能列表和表单呈现的方式。

   >[!TIP]
   >
   >查看[自定义字段类型术语表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)。

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. 输入您希望在Marketo中显示的名称。 将自动生成API名称。 您可以调整它，但设置后不能重命名它。 完成后，单击&#x200B;**创建**。

>[!CAUTION]
>
>字段名称不能开始以下字符：**&amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>SOAP API和其他后端进程使用API名称。

您现在可以在表单、流程步骤和智能列表中使用此自定义字段！
