---
unique-page-id: 1147352
description: 发送示例电子邮件 — Marketo文档 — 产品文档
title: 发送示例电子邮件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 发送示例电子邮件 {#send-a-sample-email}

发送电子邮件示例既快速又简单。 要发送动态内容电子邮件，请参阅 [预览包含动态内容的电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>您必须拥有 **Access数据库 — 运行单流操作** 发送示例电子邮件的权限。

## 发送示例电子邮件 {#send-a-sample-email-1}

1. 查找并选择您的电子邮件。 单击 **电子邮件操作** 下拉并选择 **发送示例**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >我的令牌将解析为适用于电子邮件程序的值。

1. 输入一个或多个电子邮件地址进行投放。 对于多个电子邮件地址，请使用逗号分隔。 单击 **发送** 完成时。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果您输入多个电子邮件地址，则每个收件人都会看到这些地址。 输入的第一位将是主收件人，后续的每个电子邮件地址都将是“抄送”收件人。

   >[!TIP]
   >
   >如果要以特定人员身份解析令牌，请在 **人员下拉列表** 步骤2.

## 编辑时发送示例电子邮件 {#send-a-sample-email-while-editing}

1. 查找您的电子邮件，选择它并单击 **编辑草稿** 选项卡。

   ![](assets/three-281-29.jpg)

1. 单击 **电子邮件操作**，选择 **发送示例**.

   ![](assets/four.png)

1. 输入用于投放的电子邮件地址，然后单击 **发送**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >触发器字段仅适用于以下用户： [电子邮件脚本](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting).

## 发送基于区段的示例电子邮件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[将分段应用于电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. 查找您的电子邮件，选择它并单击 **编辑草稿** 选项卡。

   ![](assets/three-281-29.jpg)

1. 单击 **预览**.

   ![](assets/1.png)

1. 单击 **查看方式** 下拉并选择 **分段**.

   ![](assets/2.png)

1. 此时将显示一个包含可用区段的下拉列表。 单击该图标并选择所需的图标。

   ![](assets/3.png)

1. 使用箭头滚动浏览您的选项（在此例中，我们动态地更改了主题行）。

   ![](assets/4.png)

1. 单击 **发送示例** 以接收正在运行的区段的测试电子邮件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您还可以在电子邮件的编辑模式下，根据区段发送示例电子邮件。 单击 **电子邮件操作** 下拉列表，选择 **发送示例**，然后选择您的区段。

在启动营销活动之前对内容进行取样非常重要。 两次测量，一次切除！
