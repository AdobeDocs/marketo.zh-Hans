---
description: 在 [!DNL Velocity Scripting] - Marketo文档 — 产品文档中更改自定义对象检索限制
title: 更改 [!DNL Velocity Scripting]中的自定义对象检索限制
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# 更改[!DNL Velocity Scripting]中的自定义对象检索限制 {#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用[!DNL Velocity Script]在电子邮件中显示自定义对象数据，则此功能可能适合您。 默认情况下，您可以从Velocity脚本访问10个父自定义对象。 如果您需要访问更多内容，请阅读。

## [!DNL Velocity]是什么 {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/)是基于[!DNL Java]构建的语言，设计用于模板化和编写HTML内容的脚本。 Marketo允许通过使用[脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)在电子邮件上下文中使用它。 通过此选项可访问存储在自定义对象中的数据。

您可以引用直接连接到Lead或Contact的父自定义对象和子自定义对象，但不能引用第三级自定义对象。 对于每个自定义对象，每个人员/联系人的10条最近更新的记录在运行时可用，并且按照从最近更新（在0时）到最旧更新（在9时）的顺序排列。

## 如何更改限制 {#how-to-change-the-limit}

1. 转到&#x200B;**[!UICONTROL 管理员]**&#x200B;部分。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 单击&#x200B;**[!UICONTROL 电子邮件]**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在[!UICONTROL 自定义对象检索限制]表中，输入新的[!UICONTROL 父检索限制]，然后单击&#x200B;**[!UICONTROL 保存更改]**。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>[!UICONTROL 父检索限制]值必须在10 - 100的范围内。 已自动为您设置[!UICONTROL 子检索限制]。 这是通过将1000除以[!UICONTROL 父检索限制]来完成的。 例如，如果将父项限制设置为50，则子项限制将变为20 (1000 ÷ 50 = 20)。

太好了！ 您现在可以从[!DNL Velocity script]访问更多自定义对象。
