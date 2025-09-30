---
unique-page-id: 2359422
description: 个性化电子邮件 – Marketo文档 – 产品文档
title: 个性化电子邮件
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '319'
ht-degree: 100%

---

# 个性化电子邮件 {#personalize-an-email}

## 任务：通过添加数据令牌，使您的电子邮件更加个性化。 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [完成设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [群发电子邮件](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [滴灌式培养](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## 步骤 1：选择一个要个性化的电子邮件 {#step-select-an-email-to-personalize}

1. 选择在[上一个快速获益](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}中创建的培养电子邮件之一，然后单击 **[!UICONTROL Create draft]**。

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >这将会创建该电子邮件的副本作为草稿。请记得批准草稿以使更改生效。

如果您未启用弹出窗口拦截器，电子邮件编辑器将会在新选项卡或新窗口中打开。否则，请连续单击两次 **[!UICONTROL Create Draft]**。

## 步骤 2：将销售人员设置为发件人 {#step-make-the-salesperson-the-sender}

1. 选择 **[!UICONTROL From]** 字段，突出显示并&#x200B;**删除**&#x200B;当前姓名。

   ![](assets/personalize-an-email-2.png)

1. 单击 **[!UICONTROL From]** 字段右侧的&#x200B;**令牌**&#x200B;图标。

   ![](assets/personalize-an-email-3.png)

1. 查找并选择 **`{{lead.Lead Owner First Name}}`** 令牌。

   ![](assets/personalize-an-email-4.png)

1. 在&#x200B;**默认值**&#x200B;中输入您的公司名称和一个破折号，以确保在销售代表名字不可用时仍显示内容。点击&#x200B;**插入**。

   ![](assets/personalize-an-email-5.png)

1. 在 **[!UICONTROL From]** 字段中按下空格键，确保光标在刚刚插入的令牌后一个空格处闪烁。然后再次单击&#x200B;**令牌**&#x200B;图标。

   ![](assets/personalize-an-email-6.png)

1. 查找并选择 **`{{lead.Lead Owner Last Name}}`** 令牌。

   ![](assets/personalize-an-email-7.png)

1. 在&#x200B;**默认值**&#x200B;中输入“销售”，然后单击&#x200B;**插入**。

   ![](assets/personalize-an-email-8.png)

## 步骤 3：将潜在客户的姓名添加到电子邮件中 {#step-add-the-leads-name-to-the-email}

1. 选择顶部可编辑区域，单击齿轮图标并选择 **[!UICONTROL Edit]**。

   ![](assets/personalize-an-email-9.png)

1. 在“您好”之后添加一个空格，将光标置于逗号前，然后单击&#x200B;**插入令牌**&#x200B;图标。

   ![](assets/personalize-an-email-10.png)

1. 查找并选择 **`{{lead.First Name}}`** 令牌。

   ![](assets/personalize-an-email-11.png)

1. 在 **[!UICONTROL Default Value]** 字段中输入“朋友”（或您希望使用的任何标签），然后单击 **[!UICONTROL Insert]**。

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >始终为令牌设置默认值；这样可以确保当部分个人信息缺失时，电子邮件中会显示默认值。

1. 单击 **[!UICONTROL Save]**。

   ![](assets/personalize-an-email-13.png)

1. 在 **[!UICONTROL Email Actions]** 下选择 **[!UICONTROL Approve and Close]**。

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速回顾如何将邮件发送给自己？请参阅[群发电子邮件](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}。

### 任务完成 {#mission-complete}

恭喜您，已成功个性化您的电子邮件！

<br> 

[◄任务 6：滴灌式培养](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任务 8：提醒销售代表 ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
