---
description: 更改中的自定义对象检索限制 [!DNL Velocity Scripting] - Marketo文档 — 产品文档”
title: 更改中的自定义对象检索限制 [!DNL Velocity Scripting]”
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# 更改中的自定义对象检索限制 [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

如果您使用 [!DNL Velocity Script] 要在电子邮件中显示自定义对象数据，可能需要使用此功能。 默认情况下，您可以从Velocity脚本访问10个父自定义对象。 如果您需要访问更多内容，请阅读。

## 什么是 [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) 是一种构建于之上的语言 [!DNL Java] 专为模板化和编写HTML内容脚本而设计。 Marketo允许它通过使用在电子邮件上下文中使用 [脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). 通过此选项可访问存储在自定义对象中的数据，以及其他内容。

您可以引用直接连接到Lead或Contact的父自定义对象和子自定义对象，但不能引用第三级自定义对象。 对于每个自定义对象，每个人员/联系人的10条最近更新的记录在运行时可用，并且按照从最近更新（在0时）到最旧更新（在9时）的顺序排列。

## 如何更改限制 {#how-to-change-the-limit}

1. 转到 **[!UICONTROL 管理员]** 部分。

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. 单击 **[!UICONTROL 电子邮件]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. 在 [!UICONTROL 自定义对象检索限制] 表格，输入新的 [!UICONTROL 父检索限制] 并单击 **[!UICONTROL 保存更改]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>此 [!UICONTROL 父检索限制] 值必须在10 - 100的范围内。 此 [!UICONTROL 子检索限制] 将自动为您设置。 这可以通过将1000除以 [!UICONTROL 父检索限制]. 例如，如果将父限制设置为50，则子限制将变为20(1000 ÷ 50 = 20)。

很好！ 您现在可以从以下位置访问更多自定义对象： [!DNL Velocity script].
