---
unique-page-id: 2360337
description: 创建和使用连接字符串（公式）字段 — Marketo文档 — 产品文档
title: 创建和使用连接字符串（公式）字段
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 创建和使用连接字符串（公式）字段 {#create-and-use-a-concatenated-string-formula-field}

您可以组合多个字段中的值，或使用Marketo公式字段构建条件值。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. 单击 **[!UICONTROL 字段管理]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. 单击 **[!UICONTROL 新建自定义字段]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. 选择 **[!UICONTROL 公式]** 对于 **[!UICONTROL 类型]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. 输入 **[!UICONTROL 名称]** ，然后单击 **[!UICONTROL 创建]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. 查找并选择公式字段，然后单击 **[!UICONTROL 编辑规则]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. 添加两个选项并像下面的屏幕快照一样定义它们。

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >详细了解 [流步骤的令牌](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. 现在，您可以在电子邮件中添加公式字段作为令牌。

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>公式字段可用于登陆页面、电子邮件和智能列表列（不导出它们）。 包含公式字段的电子邮件可以 _非_ 使用批量营销活动发送。 请使用 [电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) 在此场景中。

干得好！ 现在，你有一个智能领域，知道根据性别应该包括什么称谓。 玩得开心，发挥创意。
