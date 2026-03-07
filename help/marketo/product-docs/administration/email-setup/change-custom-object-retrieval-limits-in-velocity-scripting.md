---
description: 增加或减少电子邮件（10到100）中 [!DNL Velocity] 脚本的父自定义对象检索限制。
title: 更改 [!DNL Velocity Scripting]中的自定义对象检索限制
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# 更改[!DNL Velocity Scripting]中的自定义对象检索限制 {#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用[!DNL Velocity Script]在电子邮件中显示自定义对象数据，则此功能可能适合您。 默认情况下，您可以从Velocity脚本访问10个父自定义对象。 如果您需要访问更多内容，请阅读。

## [!DNL Velocity]是什么 {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/)是基于[!DNL Java]构建的语言，用于模板化和编写HTML内容。 Marketo允许通过使用[脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)在电子邮件上下文中使用它。 通过此选项可访问存储在自定义对象中的数据。

您可以引用直接连接到Lead或Contact的父自定义对象和子自定义对象，但不能引用第三级自定义对象。 对于每个自定义对象，每个人员/联系人的10条最近更新的记录在运行时可用，并且按照从最近更新（在0时）到最旧更新（在9时）的顺序排列。

## 如何更改限制 {#how-to-change-the-limit}

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;部分。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在[!UICONTROL Custom Object Retrieval Limits]表中，输入新的[!UICONTROL Parent Retrieval Limit]并单击&#x200B;**[!UICONTROL Save Changes]**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>[!UICONTROL Parent Retrieval Limit]值必须在10 - 100的范围内。 自动为您设置[!UICONTROL Child Retrieval Limit]。 这是通过1000除以[!UICONTROL Parent Retrieval Limit]完成的。 例如，如果将父项限制设置为50，则子项限制将变为20 (1000 ÷ 50 = 20)。

太好了！ 您现在可以从[!DNL Velocity script]访问更多自定义对象。
