---
unique-page-id: 2359416
description: 电子邮件自动响应 — Marketo Docs — 产品文档
title: 电子邮件自动响应
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 电子邮件自动响应{#email-auto-response}

## 任务：当用户填写表单{#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}时，发送感谢电子邮件

>[!PREREQUISITES]
>
>* [设置并添加人](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [登陆页表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)


## 第1步：创建电子邮件{#step-create-an-email}

1. 转到“营销活动”区域。

   ![](assets/one-2.png)

1. 选择左侧菜单中的“我的项目”，单击“新建”下拉框，然后选择“新建本地资产”。

   ![](assets/two-3.png)

1. 单击“电子邮件”。

   ![](assets/three-2.png)

1. 将您的电子邮件命名为“自动响应电子邮件”，选择模板，然后单击创建。

   ![](assets/four-1.png)

   将在新窗口或选项卡中打开电子邮件编辑器。 如果弹出窗口被阻止，请单击资产摘要页面上的&#x200B;**编辑草稿**&#x200B;以访问电子邮件。

1. 输入主题行，然后多次单击电子邮件的可编辑区域。

   ![](assets/five-2.png)

   _将在电子邮件编辑器顶部打开富文本编辑器。_

1. 突出显示现有电子邮件内容。

   ![](assets/six-2.png)

1. 键入您的电子邮件内容，然后单击“保存”。

   ![](assets/seven-2.png)

1. 您所做的更改将自动保存。 关闭电子邮件编辑器选项卡/窗口。

   ![](assets/eight-1.png)

1. 选择您的新电子邮件。 在“电子邮件操作”下，单击“批准”。

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## 第2步：创建智能活动{#step-create-a-smart-campaign}

1. 右键单击&#x200B;**我的项目**，然后单击&#x200B;**新建智能活动**。

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **将您** 的智能活动命名为“自动响应活动”，然后单击“ **创建**”。

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. 转到&#x200B;**智能列表**&#x200B;选项卡。

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   我们将设置此活动，以便当用户用Form **](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)填写您在[**&#x200B;登陆页中创建的表单时运行。

1. 找到&#x200B;**填色表单**&#x200B;触发器并将其拖动到左侧画布。

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. 在下拉列表中选择&#x200B;**我的表单**。 单击&#x200B;**Flow**&#x200B;选项卡。

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. 将&#x200B;**“发送电子邮件**”流动操作拖到左侧画布。

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. 选择&#x200B;**自动响应电子邮件**&#x200B;并转到&#x200B;**计划**&#x200B;选项卡。

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. 单击&#x200B;**编辑**。

   ![](assets/8.png)

1. 每次&#x200B;**选择**，然后单击&#x200B;**保存**。

   ![](assets/9.png)

1. 单击&#x200B;**激活**。

   ![](assets/10.png)

1. 单击确认屏幕上的&#x200B;**激活**。

   ![](assets/11.png)

>[!NOTE]
>
>激活后，此活动将在每次用户填写指定表单时运行。 活动将一直运行，直到停用为止。

## 第3步：填写{#step-fill-out-the-form}表单

1. 选择&#x200B;**我的页面**。 这是在[登陆页中创建的，Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)快速成功。

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. 单击&#x200B;**视图批准页面**。

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   您的“免费试用”登陆页将在新选项卡中打开。

1. 用您的名字、姓氏和电子邮件地址填写表单，然后单击&#x200B;**提交**。

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>确保使用实际的电子邮件地址，以便收到该电子邮件。

## 任务完成{#mission-complete}

在几分钟内，您会在收件箱中看到自动响应电子邮件。 干得好！

<br> 

[◄任务3:简单评分](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[任务5:导入潜在客户列表►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
