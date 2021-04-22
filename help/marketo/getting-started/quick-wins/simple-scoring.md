---
unique-page-id: 2359414
description: 简单评分 — Marketo文档 — 产品文档
title: 简单评分
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 简单评分{#simple-scoring}

>[!PREREQUISITES]
>
>* [设置并添加人](get-set-up-and-add-a-person.md)
>* [登陆页表单](landing-page-with-a-form.md)


## 第1步：创建评分活动{#step-create-a-scoring-campaign}

1. 转至&#x200B;**营销活动**&#x200B;区域。

   ![](assets/ma-1.png)

1. 右键单击您的&#x200B;**Learning**&#x200B;文件夹，然后单击&#x200B;**新建营销活动文件夹**。

   ![](assets/two-2.png)

1. 将活动文件夹命名为“Scorning”。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >如果您已经有一个“评分”文件夹，请将此文件夹命名为其他名称，如“评分1”。 文件夹名称必须唯一。

1. 然后右键单击新&#x200B;**Scoring**&#x200B;文件夹并选择&#x200B;**新建智能活动**。

   ![](assets/four.png)

1. **将活动** 命名为“更改得分”，然后单击“ **创建**”。

   ![](assets/five-1.png)

1. 单击&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/six-1.png)

   我们希望每当用户填写您的&#x200B;**试用申请表**&#x200B;时运行此活动。

1. 在左画布上查找并拖动&#x200B;**填色表单**&#x200B;触发器。

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. 选择&#x200B;**我的表单**。

   >[!NOTE]
   >
   >如果您用Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)快速赢取完成[登陆页，您应该有表单。 如果您为表单使用了其他名称，请选择该名称。

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. 单击&#x200B;**Flow**&#x200B;选项卡。

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. 将&#x200B;**更改分数**&#x200B;流动操作拖动到左侧画布上。

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. 您可以键入要添加到人员分数的任何值。 让我们在&#x200B;**Change**&#x200B;字段中输入“+5”。

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >良好的评分活动是为销售人员提供高质量人员的关键。 阅读&#x200B;[**潜在客户评分的最终指南**](https://www.marketo.com/definitive-guides/lead-scoring/)。

1. 单击&#x200B;**计划**&#x200B;选项卡和&#x200B;**激活**&#x200B;按钮。

   ![](assets/twelve-1.png)

1. 单击确认屏幕上的&#x200B;**激活**。

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>激活后，此活动将在每次用户填写表单时运行。 活动将一直运行，直到停用为止。

## 第2步：填写{#step-fill-out-the-form}表单

1. 选择您在[登陆页中创建的登陆页,Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)快速获胜。

   ![](assets/fourteen-1.png)

1. 单击&#x200B;**视图批准页面**。 登陆页将在新选项卡中打开。

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. 用您的名字、姓氏和电子邮件地址填写表单，然后单击&#x200B;**提交**。

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >使用您首次以个人身份输入时所用的相同名称和电子邮件地址，以应用“+5”分数增加。

## 第3步：视图人员信息{#step-view-the-person-info}

1. 转到“数据库”区域。

   ![](assets/db-2.png)

1. 搜索填写表单时使用的电子邮件地址。

   ![](assets/eighteen.png)

1. 多次单击您的人。

   ![](assets/nineteen.png)

您的人员详细信息将在新选项卡或窗口中打开。 了解填写表单时您的分数如何提高5分？!

![](assets/twenty.png)

**祝贺您！** 您创建了评分活动。[◄任务2:登陆页表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[任务4:电子邮件自动响应►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
