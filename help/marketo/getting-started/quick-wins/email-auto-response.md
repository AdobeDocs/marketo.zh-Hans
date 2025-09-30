---
unique-page-id: 2359416
description: 电子邮件自动回复 - Marketo 文档 - 产品文档
title: 电子邮件自动回复
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '340'
ht-degree: 100%

---

# 电子邮件自动回复 {#email-auto-response}

## 任务：当有人填写表单时，发送一封感谢邮件 {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [完成设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [带有表单的登陆页面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步骤 1：创建电子邮件 {#step-create-an-email}

1. 进入 [!UICONTROL Marketing Activities] 区域。

   ![](assets/email-auto-response-1.png)

1. 在左侧菜单中选择您的项目，点击 **[!UICONTROL New]** 下拉列表，并选择 **[!UICONTROL New Local Asset]**。

   ![](assets/email-auto-response-2.png)

1. 选择 **[!UICONTROL Email]**。

   ![](assets/email-auto-response-3.png)

1. 将电子邮件命名为“自动回复电子邮件”，选择一个模板，然后点击 **[!UICONTROL Create]**。

   ![](assets/email-auto-response-4.png)

   邮件编辑器将会在新窗口或选项卡中打开。如果弹出窗口被阻止，请在资产摘要页面点击 **[!UICONTROL Edit Draft]** 以访问该电子邮件。

1. 输入主题行，然后双击电子邮件中的可编辑区域。

   ![](assets/email-auto-response-5.png)

   _在电子邮件编辑器上方将打开一个富文本编辑器。_

1. 高亮选中现有的电子邮件内容。

   ![](assets/email-auto-response-6.png)

1. 输入电子邮件内容并点击 **[!UICONTROL Save]**。

   ![](assets/email-auto-response-7.png)

1. 点击 **[!UICONTROL Email Actions]** 下拉菜单，并选择 **[!UICONTROL Approve and Close]**。

   ![](assets/email-auto-response-8.png)

## 步骤 2：创建智能营销活动 {#step-create-a-smart-campaign}

1. 选择您的项目，点击 **[!UICONTROL New]** 下拉菜单，并选择 **[!UICONTROL New Smart Campaign]**。

   ![](assets/email-auto-response-9.png)

1. 将智能营销活动&#x200B;**命名为**“自动响应营销活动”，然后点击 **[!UICONTROL Create]**。

   ![](assets/email-auto-response-10.png)

1. 转到 **[!UICONTROL Smart List]** 选项卡。

   ![](assets/email-auto-response-11.png)

   我们正在设置此活动，以便在有人填写您在&#x200B;[**带有表单的登陆页面**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}&#x200B;中创建的表单时运行。

1. 找到并将 **[!UICONTROL Fills Out Form]** 触发器拖动到画布上。

   ![](assets/email-auto-response-12.png)

1. 在下拉菜单中选择 **[!UICONTROL My Form]**。单击 **[!UICONTROL Flow]** 选项卡。

   ![](assets/email-auto-response-13.png)

1. 将 **[!UICONTROL Send Email]** 流程操作拖到左侧画布。

   ![](assets/email-auto-response-14.png)

1. 选择您的&#x200B;**自动回复电子邮件**。然后点击 **[!UICONTROL Schedule]** 选项卡。

   ![](assets/email-auto-response-15.png)

1. 点击 **[!UICONTROL Edit]**。

   ![](assets/email-auto-response-16.png)

1. 选择 **[!UICONTROL every time]** 并点击 **[!UICONTROL Save]**。

   ![](assets/email-auto-response-17.png)

1. 点击 **[!UICONTROL Activate]**。

   ![](assets/email-auto-response-18.png)

1. 在确认屏幕中点击 **[!UICONTROL Activate]**。

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>激活后，该营销活动将在每次有人填写指定表单时运行。该营销活动将持续运行，直到被停用。

## 步骤 3：填写表单 {#step-fill-out-the-form}

1. 选择&#x200B;**我的页面**（此页面是在[带有表单的登陆页面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速上手任务中创建的），并点击 **[!UICONTROL Preview]**。

   ![](assets/email-auto-response-20.png)

   _您的“免费试用”登录页面将在新选项卡中打开。_

1. 填写表单中的名字、姓氏和电子邮件地址，然后点击 **[!UICONTROL Submit]**。

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>请确保使用真实的电子邮件地址，以便接收邮件。

## 任务完成 {#mission-complete}

几分钟内，您应能在收件箱中看到自动回复邮件。

[◄ 任务 3：简单评分](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[任务 5：导入人员列表 ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
