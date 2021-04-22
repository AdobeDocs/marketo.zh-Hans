---
unique-page-id: 2360337
description: 创建和使用连接字符串（公式）字段 — Marketo Docs — 产品文档
title: 创建并使用连接字符串（公式）字段
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# 创建并使用连接字符串（公式）字段{#create-and-use-a-concatenated-string-formula-field}

您可以合并多个字段的值，或使用Marketo公式字段构建条件值。

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**字段管理**。

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. 单击&#x200B;**新建自定义字段**。

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. 为&#x200B;**类型**&#x200B;选择&#x200B;**公式**。

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. 为字段输入&#x200B;**名称**，然后单击&#x200B;**创建**。

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. 查找并选择公式字段，然后单击&#x200B;**编辑规则**。

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. 添加两个选项，并像下面的屏幕截图一样定义它们。

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >了解有关流步骤[令牌的更多信息](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)。

1. 现在，您可以在电子邮件中将公式字段添加为令牌。

   ![](assets/seven.png)

>[!NOTE]
>
>公式字段可用于登陆页、电子邮件和智能列表列（不导出）。 具有公式字段的电子邮件可以&#x200B;**不能**&#x200B;使用批活动发送。 请在此方案中使用[电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)。

干得好！ 现在，您有一个智能的领域，它知道根据性别包含哪些问候。 玩得开心，尽情发挥创意。
