---
unique-page-id: 2359422
description: 个性化电子邮件 — Marketo文档 — 产品文档
title: 个性化电子邮件
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 个性化电子邮件 {#personalize-an-email}

## 任务：通过添加数据令牌使您的电子邮件个性化 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [设置并添加人员](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [发送电子邮件爆料](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [滴水，滴水，培养](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## 第1步：选择要个性化的电子邮件 {#step-select-an-email-to-personalize}

1. 选择在中创建的培养电子邮件之一 [上一个快速入门](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} 并单击 **[!UICONTROL 创建草稿]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >这会创建电子邮件的副本作为草稿。 切记批准草稿以使更改生效。

如果尚未启用弹出窗口阻止程序，则电子邮件编辑器将在新选项卡/窗口中打开。 否则，请单击 **[!UICONTROL 创建草稿]** 两次。

## 步骤2：使销售人员成为发件人 {#step-make-the-salesperson-the-sender}

1. 选择 **[!UICONTROL 起始日期]** 字段，突出显示和 **delete** 当前名称。

   ![](assets/personalize-an-email-2.png)

1. 单击 **令牌** 图标右侧的 **[!UICONTROL 起始日期]** 字段。

   ![](assets/personalize-an-email-3.png)

1. 查找并选择 **`{{lead.Lead Owner First Name}}`** 令牌。

   ![](assets/personalize-an-email-4.png)

1. 键入您的公司名称和短划线 **默认值** 以确保在销售代表的名字不可用时显示某些内容。 单击 **插入**.

   ![](assets/personalize-an-email-5.png)

1. 点击中的空格键 **[!UICONTROL 起始日期]** 字段，确保光标在您刚刚插入的令牌后闪烁一个空格。 然后单击 **令牌** 图标。

   ![](assets/personalize-an-email-6.png)

1. 查找并选择 **`{{lead.Lead Owner Last Name}}`** 令牌。

   ![](assets/personalize-an-email-7.png)

1. 键入“Sales”作为 **默认值** 并单击 **插入**.

   ![](assets/personalize-an-email-8.png)

## 步骤3：将商机的名称添加到电子邮件中 {#step-add-the-leads-name-to-the-email}

1. 选择顶部可编辑部分，单击齿轮图标并选择 **[!UICONTROL 编辑]**.

   ![](assets/personalize-an-email-9.png)

1. 在“Hello”后添加空格，并将光标放在逗号前面，然后单击 **插入令牌** 图标。

   ![](assets/personalize-an-email-10.png)

1. 查找并选择 **`{{lead.First Name}}`** 令牌。

   ![](assets/personalize-an-email-11.png)

1. 在“ ”中输入“Friend”（或任何您想要的标签） **[!UICONTROL 默认值]** 字段并单击 **[!UICONTROL 插入]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >始终包含令牌的默认值；这可确保在部分个人信息缺失时，电子邮件中会显示默认值。

1. 单击 **[!UICONTROL 保存]**.

   ![](assets/personalize-an-email-13.png)

1. 下 **[!UICONTROL 电子邮件操作]** 并选择 **[!UICONTROL 批准并关闭]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>需要快速了解如何发送电子邮件给您自己？ 参见 [发送电子邮件爆料](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### 任务完成 {#mission-complete}

恭喜，您已个性化您的电子邮件！

<br> 

[◄任务6：滴水、滴水、Nurture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[任务8：提醒销售代表►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
