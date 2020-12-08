---
unique-page-id: 2359422
description: 个性化电子邮件——营销文档——产品文档
title: 个性化电子邮件
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# 个性化电子邮件 {#personalize-an-email}

## 任务：通过添加数据令牌，使您的电子邮件个性化 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**先决条件**
>
>* [设置并添加人物](get-set-up-and-add-a-person.md)
>* [发送电子邮件爆炸](send-an-email.md)
>* [滴水，滴水，培养](drip-drip-nurture.md)


## 第1步：选择要个性化的电子邮件 {#step-select-an-email-to-personalize}

1. 选择在上一个快速赢取中创建的培养电 [子邮件之一](drip-drip-nurture.md) ，然后单 **击“编辑草稿”**。

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >这将创建电子邮件副本作为草稿。 您必须批准草稿，更改才能生效。

   **编辑草稿**

如果尚未启用弹出窗口阻止程序，则电子邮件编辑器将在新的选项卡／窗口中打开。 否则，单击两次。

## 第2步：让销售人员成为发件人 {#step-make-the-salesperson-the-sender}

1. 选择“ **发件人** ”字段，高亮 **并删** 除当前的名称。

   ![](assets/two-5.png)

1. 单击 **“发件人** ”字段右侧的“ **令牌** ”。

   ![](assets/three-4.png)

1. 查找并选择 **`{{lead.Lead Owner First Name}}`** 令牌。

   ![](assets/four-3.png)

1. 键入公司名和“默认值 **”短划线** ，确保在销售代表的名字不可用时显示某些内容。 单击 **插入**。

   ![](assets/five-4.png)

1. 点击“发件人”字 **段中** 的空格栏，确保光标在刚刚插入的标记后闪烁一个空格。 然后再次单 **击令牌** 图标。

   ![](assets/six-4.png)

1. 查找并选择 **`{{lead.Lead Owner Last Name}}`** 令牌。

   ![](assets/seven-5.png)

1. 键入“Sales”作为默认 **值** ，然后单 **击Insert**。

   ![](assets/eight-3.png)

## 第3步：将潜在客户姓名添加到电子邮件 {#step-add-the-leads-name-to-the-email}

1. 选择顶部的可编辑部分，单击齿轮图标，然后选择“ **编辑**”。

   ![](assets/nine-2.png)

1. 在“Hello”后添加一个空格，将光标放在逗号前面，然后单击“插入 **令牌** ”图标。

   ![](assets/ten-4.png)

1. 查找并选择 **`{{lead.First Name}}`** 令牌。

   ![](assets/eleven-4.png)

1. 在“默认值”字段中输入“朋友”(或您喜欢的任何标 **签)** ，然后单击“ **插入”**。

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >始终包含令牌的默认值；这可确保在缺少部分个人信息时，电子邮件中显示默认值。

1. 单击 **保存**。

   ![](assets/thirteen-3.png)

1. 关闭电子邮件编辑器选项卡／窗口。

   ![](assets/fourteen-3.png)

1. 在“电 **子邮件操作**”下，选 **择“批准草稿**”。

   ![](assets/fifteen-3.png)

>[!TIP]
>
>需要快速复习一下如何给自己发送电子邮件的方法？ 请参 [阅发送电子邮件爆炸](send-an-email.md)。

### 观看视频 {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/iRnqxMyJg6VKyuPeuxmHFb.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

### 任务完成 {#mission-complete}

祝贺您，您的电子邮件已个性化！

<br> 

[◄任务6:滴滴，滴滴，培养](drip-drip-nurture.md)[使命8:提醒销售代表►](alert-the-sales-rep.md)