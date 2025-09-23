---
unique-page-id: 2360337
description: 创建并使用连接字符串（公式）字段 — Marketo文档 — 产品文档
title: 创建并使用连接字符串（公式）字段
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 13%

---

# 创建并使用连接字符串（公式）字段 {#create-and-use-a-concatenated-string-formula-field}

您可以组合多个字段中的值，或使用Marketo Engage公式字段构建条件值。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. 单击 **[!UICONTROL Field Management]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. 单击 **[!UICONTROL New Custom Field]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. 为&#x200B;**[!UICONTROL Formula]**&#x200B;选择&#x200B;**[!UICONTROL Type]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. 为您的字段输入&#x200B;**[!UICONTROL Name]**，然后单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. 查找并选择公式字段，然后单击&#x200B;**[!UICONTROL Edit Rules]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. 添加两个选项并像下面的屏幕快照一样定义它们。

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >了解有关流程步骤[的](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)令牌的更多信息。

1. 现在，您可以在电子邮件中添加公式字段作为令牌。

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>公式字段可用于登陆页面、电子邮件和智能列表列。 带有公式字段的电子邮件&#x200B;_不能_&#x200B;使用批处理营销活动发送。 请在此方案中使用[电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)。

做得好！ 现在，你有一个聪明的领域，知道根据性别应该包括什么称谓。 玩得开心，发挥创意。
