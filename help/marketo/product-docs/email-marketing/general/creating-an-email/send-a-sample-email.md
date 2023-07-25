---
unique-page-id: 1147352
description: 发送示例电子邮件 — Marketo文档 — 产品文档
title: 发送示例电子邮件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 发送示例电子邮件 {#send-a-sample-email}

发送电子邮件示例既快速又简单。 要发送动态内容电子邮件，请参阅 [预览包含动态内容的电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>您必须拥有 **Access数据库 — 运行单流操作** 发送示例电子邮件的权限。

## 发送示例电子邮件 {#send-a-sample-email-1}

1. 查找并选择您的电子邮件。 单击 **电子邮件操作** 下拉菜单并选择 **发送示例**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >我的令牌解析为适用于电子邮件程序的值。

1. 输入一个或多个要投放的电子邮件地址。 对于多个电子邮件地址，请使用逗号分隔它们。 单击 **发送** 完成时。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果您输入多个电子邮件地址，则每个收件人都会看到这些地址。 输入的第一个电子邮件地址将是主收件人，后续的每个电子邮件地址都将是“抄送”收件人。

   >[!TIP]
   >
   >如果要将令牌解析为特定人员，请在 **人员下拉列表** 步骤2.

## 编辑时发送示例电子邮件 {#send-a-sample-email-while-editing}

1. 找到您的电子邮件，将其选中并单击 **编辑草稿** 选项卡。

   ![](assets/three-281-29.jpg)

1. 单击 **电子邮件操作**，选择 **发送示例**.

   ![](assets/four.png)

1. 输入投放的电子邮件地址，然后单击 **发送**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >触发器字段仅适用于那些利用 [电子邮件脚本](https://developers.marketo.com/documentation/velocity-script/).

## 发送基于区段的示例电子邮件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[将分段应用于您的电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. 找到您的电子邮件，将其选中并单击 **编辑草稿** 选项卡。

   ![](assets/three-281-29.jpg)

1. 单击 **预览**.

   ![](assets/1.png)

1. 单击 **查看方式** 下拉菜单并选择 **分段**.

   ![](assets/2.png)

1. 此时将显示一个下拉列表，其中包含可用的分段。 单击该图标并选择所需的图标。

   ![](assets/3.png)

1. 使用箭头滚动浏览您的选项（在此例中，我们动态地更改了主题行）。

   ![](assets/4.png)

1. 单击 **发送示例** 以接收正在运行的区段的测试电子邮件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您还可以在电子邮件的编辑模式下，根据区段发送示例电子邮件。 单击 **电子邮件操作** 下拉列表，选择 **发送示例**，然后选择您的区段。

在启动营销活动之前对内容进行取样非常重要。 两次测量，一次切除！
