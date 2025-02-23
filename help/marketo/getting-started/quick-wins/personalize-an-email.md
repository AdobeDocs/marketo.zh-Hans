---
unique-page-id: 2359422
description: 个性化电子邮件 — Marketo文档 — 产品文档
title: 电子邮件个性化
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 电子邮件个性化 {#personalize-an-email}

## 任务：通过添加数据令牌使您的电子邮件个性化 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [发送电子邮件爆炸邮件](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [滴水，滴水，培养](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## 第1步：选择要个性化的电子邮件 {#step-select-an-email-to-personalize}

1. 选择在[上一个快速入门](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}中创建的培养电子邮件之一，然后单击&#x200B;**[!UICONTROL 创建草稿]**。

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >这会创建电子邮件的副本作为草稿。 请记得批准草稿，以便更改生效。

如果尚未启用弹出窗口阻止程序，则将在一个新的选项卡/窗口中打开电子邮件编辑器。 否则，单击&#x200B;**[!UICONTROL 创建草稿]**&#x200B;两次。

## 第2步：使销售人员成为发件人 {#step-make-the-salesperson-the-sender}

1. 选择&#x200B;**[!UICONTROL From]**&#x200B;字段，突出显示并&#x200B;**删除**&#x200B;当前名称。

   ![](assets/personalize-an-email-2.png)

1. 单击&#x200B;**[!UICONTROL 从]**&#x200B;字段右侧的&#x200B;**令牌**&#x200B;图标。

   ![](assets/personalize-an-email-3.png)

1. 查找并选择&#x200B;**`{{lead.Lead Owner First Name}}`**&#x200B;令牌。

   ![](assets/personalize-an-email-4.png)

1. 键入您的公司名称和&#x200B;**默认值**&#x200B;的短划线，以确保在销售代表的名字不可用时显示某些内容。 单击&#x200B;**插入**。

   ![](assets/personalize-an-email-5.png)

1. 点击&#x200B;**[!UICONTROL 从]**&#x200B;字段中的空格键，确保光标在您刚刚插入的令牌后闪烁一个空格。 然后再次单击&#x200B;**令牌**&#x200B;图标。

   ![](assets/personalize-an-email-6.png)

1. 查找并选择&#x200B;**`{{lead.Lead Owner Last Name}}`**&#x200B;令牌。

   ![](assets/personalize-an-email-7.png)

1. 为&#x200B;**默认值**&#x200B;键入“Sales”，然后单击&#x200B;**插入**。

   ![](assets/personalize-an-email-8.png)

## 步骤3：将商机的名称添加到电子邮件中 {#step-add-the-leads-name-to-the-email}

1. 选择顶部可编辑部分，单击齿轮图标并选择&#x200B;**[!UICONTROL 编辑]**。

   ![](assets/personalize-an-email-9.png)

1. 在“Hello”后添加空格，并将光标放在逗号前面，然后单击&#x200B;**插入令牌**&#x200B;图标。

   ![](assets/personalize-an-email-10.png)

1. 查找并选择&#x200B;**`{{lead.First Name}}`**&#x200B;令牌。

   ![](assets/personalize-an-email-11.png)

1. 在&#x200B;**[!UICONTROL 默认值]**&#x200B;字段中输入“Friend”（或任何所需的标签），然后单击&#x200B;**[!UICONTROL 插入]**。

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >始终包含令牌的默认值；如果部分个人信息缺失，这将确保默认值在电子邮件中显示。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/personalize-an-email-13.png)

1. 在&#x200B;**[!UICONTROL 电子邮件操作]**&#x200B;下，选择&#x200B;**[!UICONTROL 批准并关闭]**。

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速刷新一下如何发送电子邮件？ 请参阅[发送电子邮件爆炸邮件](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}。

### 任务完成 {#mission-complete}

恭喜，您已个性化您的电子邮件！

<br> 

[◄任务6：滴水、滴水、培养](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任务8：提醒销售代表►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
