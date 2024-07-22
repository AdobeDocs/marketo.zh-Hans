---
description: 全局表单验证规则 — Marketo文档 — 产品文档
title: 全局表单验证规则
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 全局表单验证规则 {#global-form-validation-rules}

此功能允许您阻止特定域提交到Marketo Engage表单。

## 如何启用访问 {#how-to-enable-access}

在您可以使用此功能之前，必须为每个所需角色启用其权限。

1. 在Marketo中，单击&#x200B;**[!UICONTROL 管理员]**。

   ![](assets/global-form-validation-rules-1.png)

1. 单击&#x200B;**[!UICONTROL 用户和角色]**。

   ![](assets/global-form-validation-rules-2.png)

1. 单击&#x200B;**[!UICONTROL 角色]**&#x200B;选项卡。

   ![](assets/global-form-validation-rules-3.png)

1. 双击要向其授予权限的角色。

   ![](assets/global-form-validation-rules-4.png)

1. 单击“访问管理员”旁边的&#x200B;**+**&#x200B;号。

   ![](assets/global-form-validation-rules-5.png)

1. 向下滚动并选择&#x200B;**[!UICONTROL 访问表单验证规则]**，然后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/global-form-validation-rules-6.png)

## 创建新表单验证规则 {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>这些规则将适用于您的Marketo Engage订阅中的所有表单。

1. 在Marketo中，单击&#x200B;**[!UICONTROL 管理员]**。

   ![](assets/global-form-validation-rules-7.png)

1. 单击&#x200B;**[!UICONTROL 全局表单验证规则]**。

   ![](assets/global-form-validation-rules-8.png)

1. 单击&#x200B;**[!UICONTROL 新建表单验证规则]**。

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >表单验证规则操作下拉列表允许您删除或编辑现有规则。

1. 命名规则，为其提供可选描述，然后输入您希望表单访客看到的错误消息。 在规则框中输入要阻止的域，选择&#x200B;**[!UICONTROL 激活规则]**，然后单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage定义了免费消费者电子邮件域的阻止列表 列入阻止列表，在使用我们预加载的“消费者电子邮件域”规则时，将阻止这些域。 [在此查看该列表](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv)。

## 如何禁用每个表单的访问权限{#how-to-disable-access-per-form}

启用后，规则将应用于所有表单。 但是，如果您有一个具有特定要求的表单，并且您不希望任何内容被拒绝，则可以在表单的设置中禁用[!UICONTROL 全局表单验证规则]。

1. 在所需表单中，单击&#x200B;**[!UICONTROL 表单设置]**，然后单击&#x200B;**[!UICONTROL 设置]**。

   ![](assets/global-form-validation-rules-11.png)

1. 单击&#x200B;**[!UICONTROL 全局表单验证规则]**&#x200B;下拉列表，然后选择&#x200B;**[!UICONTROL 已禁用]**。

   ![](assets/global-form-validation-rules-12.png)

当您批准并发布表单时，它将忽略您的[!UICONTROL 全局表单验证规则]。
