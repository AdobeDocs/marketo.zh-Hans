---
unique-page-id: 2359414
description: 简单评分 — Marketo文档 — 产品文档
title: 简单评分
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 简单评分 {#simple-scoring}

>[!PREREQUISITES]
>
>* [设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* 带有表单的[登陆页面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步骤1：创建评分营销活动 {#step-create-a-scoring-campaign}

1. 转到&#x200B;**[!UICONTROL 营销活动]**&#x200B;区域。

   ![](assets/simple-scoring-1.png)

1. 右键单击您的&#x200B;**学习**&#x200B;文件夹，然后单击&#x200B;**[!UICONTROL 新建Campaign文件夹]**。

   ![](assets/simple-scoring-2.png)

1. 将营销活动文件夹命名为“评分”，然后单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >如果您已经有一个评分文件夹，请将其命名为其他名称，例如评分1。 文件夹名称必须是唯一的。

1. 右键单击您的&#x200B;**评分**&#x200B;文件夹并选择&#x200B;**[!UICONTROL 新建智能营销活动]**。

   ![](assets/simple-scoring-4.png)

1. 将营销活动命名为“更改得分”，然后单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/simple-scoring-5.png)

1. 单击&#x200B;**[!UICONTROL 智能列表]**&#x200B;选项卡。

   ![](assets/simple-scoring-6.png)

   我们希望每当有人填写您的&#x200B;**试用申请表**&#x200B;时运行此营销活动。

1. 查找&#x200B;**[!UICONTROL 填写表单]**&#x200B;触发器并将其拖动到左画布上。

   ![](assets/simple-scoring-7.png)

1. 选择&#x200B;**我的表单**。

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >如果您使用表单[&#128279;](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速入选完成了登陆页面，则您应该拥有表单。 如果表单使用了其他名称，请选择该名称。

1. 单击&#x200B;**[!UICONTROL 流量]**&#x200B;选项卡。

   ![](assets/simple-scoring-9.png)

1. 将&#x200B;**更改得分**&#x200B;流程操作拖动到左画布上。

   ![](assets/simple-scoring-10.png)

1. 您可以键入要添加到人员得分的任何值。 让我们在&#x200B;**[!UICONTROL 更改]**&#x200B;字段中输入“+5”。

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >良好的评分活动是向销售人员提供高质量人员的关键。 阅读&#x200B;[**引导评分的最终指南**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}。

1. 单击&#x200B;**[!UICONTROL 计划]**&#x200B;选项卡和&#x200B;**[!UICONTROL 激活]**&#x200B;按钮。

   ![](assets/simple-scoring-12.png)

1. 在确认屏幕上单击&#x200B;**[!UICONTROL 激活]**。

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>一旦激活，此营销活动将在每次用户填写表单时运行。 该营销活动将继续运行，直到被停用。

## 第2步：填写表单 {#step-fill-out-the-form}

1. 选择您在[登录页面中创建的带有表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}的登录页面。

   ![](assets/simple-scoring-14.png)

1. 单击&#x200B;**[!UICONTROL 预览]**。 登陆页面将在新选项卡中打开。

   ![](assets/simple-scoring-15.png)

1. 填写您的名字、姓氏和电子邮件地址，然后单击&#x200B;**[!UICONTROL 提交]**。

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >使用您首次以个人身份输入时所用的相同名称和电子邮件地址，以应用“+5”分数提升。

## 步骤3：查看人员信息 {#step-view-the-person-info}

1. 转到&#x200B;**[!UICONTROL 数据库]**&#x200B;区域。

   ![](assets/simple-scoring-17.png)

1. 搜索您在填写表单时使用的电子邮件地址。

   ![](assets/simple-scoring-18.png)

1. 双击您的人员。

   ![](assets/simple-scoring-19.png)

将在新选项卡或窗口中打开您的人员详细信息。 了解填写表单后得分如何提高5分？

![](assets/simple-scoring-20.png)

## 任务完成！ {#mission-complete}

<br> 

[◄任务2：带有表单的登陆页面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[任务4：电子邮件自动响应►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
