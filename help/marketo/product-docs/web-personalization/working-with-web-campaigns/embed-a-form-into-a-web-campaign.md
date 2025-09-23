---
unique-page-id: 10095554
description: 将表单嵌入到Web营销活动 — Marketo文档 — 产品文档
title: 将表单嵌入 Web 营销活动
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 8%

---

# 将表单嵌入 Web 营销活动 {#embed-a-form-into-a-web-campaign}

了解如何将Marketo表单嵌入到Web营销活动中（对话框、区域或小部件）。

1. 右键单击已批准的表单。 选择 **[!UICONTROL Embed Code]**。

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. 复制代码。

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. 在[!DNL Web Personalization]中，转到&#x200B;**[!UICONTROL Web Campaigns]**。

   ![](assets/web-campaigns-hand-7.jpg)

1. 单击 **[!UICONTROL Create New Campaign]**。

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. 在富文本编辑器中，单击HTML图标。

   ![](assets/five-1.png)

1. 将表单嵌入代码粘贴到[!UICONTROL HTML Source Editor]中。 单击 **[!UICONTROL Update]**。

   ![](assets/six-1.png)

1. 该表单将不会显示在编辑器视图中，但您可以预览它以查看它在营销活动中的呈现方式。

1. 单击&#x200B;**[!UICONTROL Launch]**&#x200B;启动营销活动。

   >[!NOTE]
   >
   >对表单字段的任何更改必须在编辑表单草稿的Marketo营销活动中完成。

## 将背景图像添加到表单的三种方法 {#three-ways-to-add-a-background-image-to-a-form}

要将背景图像添加到表单，您可以：

* 编辑表单主题的 CSS
* 在Set Campaign中更改对话框或构件颜色
* 将CSS代码添加到脚本中

要编辑表单主题的CSS，请参阅[本文](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)。

要在Set Campaign中更改对话框或小组件颜色，请执行以下操作：

1. 在富文本编辑器中，选择对话框营销活动类型和对话框样式、标题颜色和背景颜色，以自定义表单的背景颜色。 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. 以下示例展示了带有浅紫色标题和背景颜色的“现代修剪”对话框样式的外观。

   ![](assets/image2015-12-29-18-3a27-3a31.png)

要将CSS代码添加到脚本，请执行以下操作：

1. 在富文本编辑器中，单击HTML图标。

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. 将带有背景样式代码的表单嵌入代码粘贴到[!UICONTROL HTML Source Editor]中。 单击 **[!UICONTROL Update]**。

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. 单击&#x200B;**[!UICONTROL Preview]**&#x200B;查看它在营销活动中的呈现方式（该表单不会显示在编辑器视图中）。 以下示例介绍了上述表单代码如何在具有背景图像的营销活动中呈现。

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [编辑表单主题的CSS](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [显示没有后续登陆页面的感谢消息](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Forms 2.0](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
