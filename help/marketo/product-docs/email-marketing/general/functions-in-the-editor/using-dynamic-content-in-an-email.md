---
unique-page-id: 2950617
description: 在电子邮件中使用动态内容 — Marketo文档 — 产品文档
title: 在电子邮件中使用动态内容
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 4%

---

# 在电子邮件中使用动态内容 {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[创建分段](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

在电子邮件中使用动态内容发送商机目标信息。

>[!NOTE]
>
>仅当使用“触发营销活动”时，才支持在电子邮件中的动态内容中使用变量。 使用批量营销活动时&#x200B;**不支持**。

## 添加分段 {#add-segmentation}

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/login-marketing-activities.png)

1. 选择您的电子邮件并单击&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/1.2.png)

1. 在本例中，我们将使“主题行”成为动态的。 单击[!UICONTROL Subject]字段，然后单击&#x200B;**生成动态**&#x200B;按钮。

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >您还可以使电子邮件中的元素成为动态元素。 为此，请选择该区域，单击齿轮图标，然后选择&#x200B;**生成动态**（或[替换为代码片段](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md)，具体取决于您正在执行的操作）。

1. 输入分段名称，将其选定，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/1.4.png)

   您的分段及其分段显示在右侧的[!UICONTROL Dynamic]选项卡下。

   ![](assets/1.5.png)

## 应用动态内容 {#apply-dynamic-content}

>[!CAUTION]
>
>允许的动态内容元素数量不受限制。 虽然没有特定的数量限制（它可能因内容组合而异），但过度使用动态内容可能会对电子邮件的性能产生负面影响。 我们建议将每封电子邮件使用的动态内容元素数量保持在20个以下。

1. 单击区段并添加主题行。

![](assets/2.1.png)

1. 对每个区段重复执行上述步骤。

   ![](assets/2.2.png)

>[!TIP]
>
>在将内容应用于各种区段之前，请创建默认电子邮件。

>[!CAUTION]
>
>对默认区段内容块所做的更改将应用于所有区段。

真贴心！ 现在，您可以向目标受众发送灵活的电子邮件。

>[!MORELIKETHIS]
>
>* [预览包含动态内容的电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [在登陆页面中使用动态内容](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
