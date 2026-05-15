---
unique-page-id: 2360337
description: 组合多个字段中的值或使用Marketo Engage中的公式字段构建条件值。
title: 创建并使用串联字符串（公式）字段
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
TQID: https://experienceleague.adobe.com/Yk-Xh-WHUE8-GR2KTCxXRSqerdz-JHu2JnzYp8tAq9U
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 136
ht-degree: 0%

---

# 创建并使用串联字符串（公式）字段 {#create-and-use-a-concatenated-string-formula-field}

您可以组合多个字段中的值，或使用Marketo Engage公式字段构建条件值。

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域。

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. 单击&#x200B;**[!UICONTROL Field Management]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. 单击&#x200B;**[!UICONTROL New Custom Field]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. 为&#x200B;**[!UICONTROL Type]**&#x200B;选择&#x200B;**[!UICONTROL Formula]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. 为您的字段输入&#x200B;**[!UICONTROL Name]**，然后单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. 查找并选择公式字段，然后单击&#x200B;**[!UICONTROL Edit Rules]**。

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. 添加两个选项并像下面的屏幕快照一样定义它们。

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >了解有关流程步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)的[令牌的更多信息。

1. 现在，您可以在电子邮件中添加公式字段作为令牌。

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>公式字段可用于登陆页面、电子邮件和智能列表列。 带有公式字段的电子邮件&#x200B;_不能_&#x200B;使用批处理营销活动发送。 在此方案中使用[电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)。
