---
unique-page-id: 2359412
description: 带表单的登陆页面 — Marketo文档 — 产品文档
title: 带有表单的登陆页面
exl-id: 4ae6df7c-96d0-4bfe-962c-e14ecb877a6a
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 7%

---

# 带有表单的登陆页面 {#landing-page-with-a-form}

## 任务：创建一个带有表单的登陆页面，以吸引新人员。 {#mission-create-a-landing-page-with-a-form-to-acquire-new-people}

>[!PREREQUISITES]
>
>[完成设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

## 第1步：创建程序 {#step-create-a-program}

1. 进入 **[!UICONTROL Marketing Activities]** 区域。

   ![](assets/landing-page-with-a-form-1.png)

1. 选择在&#x200B;**上一个快速入门**&#x200B;中创建的[学习](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}文件夹。 在&#x200B;**[!UICONTROL New]**&#x200B;下，单击&#x200B;**[!UICONTROL New Program]**。

   ![](assets/landing-page-with-a-form-2.png)

1. 输入程序&#x200B;**[!UICONTROL Name]**，选择&#x200B;**[!UICONTROL Channel]**，然后单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/landing-page-with-a-form-3.png)

   >[!TIP]
   >
   >在项目名称的末尾包含您的缩写以使其唯一。

   >[!NOTE]
   >
   >项目是一项特定的营销计划。 **渠道**&#x200B;旨在作为投放机制，如网络研讨会、赞助或在线广告。 根据您自己的实例中提供的内容，您可能会在下拉列表中看到不同的渠道选项。 您也可以[创建自己的频道](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}。

做得好！ 现在，我们已经创建了一个项目，接下来让我们创建一些内容。

## 第2步：创建表单 {#step-create-a-form}

1. 选择项目后，单击&#x200B;**[!UICONTROL New]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/landing-page-with-a-form-4.png)

1. 选择 **[!UICONTROL Form]**。

   ![](assets/landing-page-with-a-form-5.png)

1. 输入表单&#x200B;**[!UICONTROL Name]**&#x200B;并单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/landing-page-with-a-form-6.png)

   >[!NOTE]
   >
   >确保选中&#x200B;**[!UICONTROL Open in editor]**&#x200B;框。 如果不是，则需要单击&#x200B;**[!UICONTROL Edit Form]**&#x200B;选项卡。

   >[!TIP]
   >
   >看不到表单编辑器？ 您的浏览器可能阻止了窗口。 在浏览器中启用`app.marketo.com`中的弹出窗口，然后单击顶部菜单栏中的编辑草稿。

1. 选择&#x200B;**[!UICONTROL Email Address]**&#x200B;字段并选中&#x200B;**[!UICONTROL Is Required]**。

   ![](assets/landing-page-with-a-form-7.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/landing-page-with-a-form-8.png)

1. 单击箭头可滚动浏览主题。 选择一个。

   ![](assets/landing-page-with-a-form-9.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/landing-page-with-a-form-10.png)

1. 在“感谢页面”部分下，为&#x200B;**[!UICONTROL External URL]**&#x200B;选择&#x200B;**[!UICONTROL Follow Up With]**。

   ![](assets/landing-page-with-a-form-11.png)

1. 输入URL。

   ![](assets/landing-page-with-a-form-12.png)

   >[!NOTE]
   >
   >“跟进”页面是在填写表单后重定向访客的位置。 外部URL是一个选项，但还有更多选项。 请参阅[设置表单感谢页面](/help/marketo/product-docs/demand-generation/forms/creating-a-form/set-a-form-thank-you-page.md){target="_blank"}。

1. 单击 **[!UICONTROL Finish]**。

   ![](assets/landing-page-with-a-form-13.png)

1. 单击 **[!UICONTROL Approve and Close]**。

   ![](assets/landing-page-with-a-form-14.png)

   太棒了！ 现在，您有一个包含表单的程序。 让我们继续并创建页面。

## 第3步：创建登陆页面并添加表单 {#step-create-a-landing-page-and-add-your-form}

1. 选择项目后，单击&#x200B;**[!UICONTROL New]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/landing-page-with-a-form-15.png)

1. 选择 **[!UICONTROL Landing Page]**。

   ![](assets/landing-page-with-a-form-16.png)

1. 输入页面&#x200B;**[!UICONTROL Name]**，选择模板并单击&#x200B;**[!UICONTROL Create]**。

   >[!NOTE]
   >
   >您可能有不同的模板，不同于屏幕快照中的模板，没关系，只要选择一个模板并继续操作即可。

   ![](assets/landing-page-with-a-form-17.png)

1. 打开登陆页面编辑器后，将[!UICONTROL Form]元素拖动到画布上。

   ![](assets/landing-page-with-a-form-18.png)

1. 查找并选择您的表单，然后单击&#x200B;**[!UICONTROL Insert]**。

   ![](assets/landing-page-with-a-form-19.png)

1. 将表单拖动到所需的位置。

   ![](assets/landing-page-with-a-form-20.png)

1. 所有更改都将自动保存。 关闭表单编辑器选项卡/窗口。

   ![](assets/landing-page-with-a-form-21.png)

   做得好！现在，您有一个登陆页面，上面有一个表单。 让我们批准您的页面以使其上线。

## 第4步：批准您的登陆页面 {#step-approve-your-landing-page}

1. 选择您的登陆页面并单击&#x200B;**[!UICONTROL Approve draft]**。

   ![](assets/landing-page-with-a-form-22.png)

   >[!NOTE]
   >
   >批准登陆页面后，即可使其上线并可在Internet上访问。

   完美！ 看到上面绿色的复选标记了吗？

   ![](assets/landing-page-with-a-form-23.png)

## 步骤5：测试表单 {#step-test-your-form}

1. 选择您的登陆页面并单击&#x200B;**[!UICONTROL View Approved Page]**。

   ![](assets/landing-page-with-a-form-24.png)

1. 使用您知道唯一的信息填写表单，然后单击&#x200B;**[!UICONTROL Submit]**。

   ![](assets/landing-page-with-a-form-25.png)

1. 进入 **[!UICONTROL Database]** 区域。

   ![](assets/landing-page-with-a-form-26.png)

1. 搜索您在填写表单时使用的唯一电子邮件地址。

   ![](assets/landing-page-with-a-form-27.png)

   就在这儿！ 您创建了一个带有表单的新登陆页面，并使用它生成了一个新人员。

   ![](assets/landing-page-with-a-form-28.png)

## 任务完成！ {#mission-complete}

<br> 

[◄任务1：发送电子邮件爆炸邮件](/help/marketo/getting-started/quick-wins/send-an-email.md)

[任务3：简单得分►](/help/marketo/getting-started/quick-wins/simple-scoring.md)
