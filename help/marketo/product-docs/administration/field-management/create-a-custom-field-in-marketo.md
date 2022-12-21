---
unique-page-id: 2360287
description: 在Marketo - Marketo文档 — 产品文档中创建自定义字段
title: 在Marketo中创建自定义字段
exl-id: 6face1d7-6a4e-412b-9708-6aa7e43e8c11
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# 在Marketo中创建自定义字段 {#create-a-custom-field-in-marketo}

如果您需要在Marketo中新建一个自定义字段来存储/捕获数据，请参阅以下如何创建一个字段。

1. 转到“管理员”并单击 **字段管理**.

   ![](assets/image2014-9-24-13-3a46-3a26.png)

   >[!TIP]
   >
   >如果您希望这些字段与CRM保持同步，请在CRM中创建它们，之后将在Marketo中自动创建它们。

1. 单击 **新建自定义字段**.

   ![](assets/two.png)

1. 选择字段类型。 这将更改它在Marketo中智能列表和表单中的呈现方式。

   >[!TIP]
   >
   >查看 [自定义字段类型术语表](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

   ![](assets/image2014-9-24-13-3a47-3a42.png)

1. 输入您希望在Marketo中显示的名称。 API名称将自动生成。 您可以对其进行调整，但设置后便无法对其重命名。 单击 **创建** 完成时。

>[!CAUTION]
>
>字段名称不能以以下字符开头： **.&amp; +[]**

![](assets/image2014-9-24-13-3a48-3a26.png)

>[!NOTE]
>
>SOAP API和其他后端进程会使用API名称。

您现在可以在表单、流程步骤和智能列表中使用此自定义字段！
