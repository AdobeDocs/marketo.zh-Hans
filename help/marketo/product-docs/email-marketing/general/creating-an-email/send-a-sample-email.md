---
unique-page-id: 1147352
description: 发送示例电子邮件 — Marketo文档 — 产品文档
title: 发送示例电子邮件
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
source-git-commit: 1586b71ec9f9c4f8abc4fd9a3277d5a5f5b88080
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 发送示例电子邮件 {#send-a-sample-email}

发送电子邮件的样本既快捷又简单。 要发送动态内容电子邮件，请参阅 [预览包含动态内容的电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>您必须拥有 **访问数据库 — 运行单个流操作** 发送示例电子邮件的权限。

## 发送示例电子邮件 {#send-a-sample-email-1}

1. 查找并选择您的电子邮件。 单击 **电子邮件操作** 下拉框并选择 **发送示例**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >我的令牌可解析为适用于电子邮件程序的值。

1. 输入一个或多个要投放的电子邮件地址。 对于多个电子邮件地址，请使用逗号分隔它们。 单击 **发送** 完成时。

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >如果输入多个电子邮件地址，则每个收件人都可以看到这些地址。 输入的第一个收件人将是主收件人，每个后续电子邮件地址都将是抄送收件人。

   >[!TIP]
   >
   >如果要将令牌解析为特定人员，请在 **“人员”下拉列表** 中，选择要删除的数据。

## 编辑时发送示例电子邮件 {#send-a-sample-email-while-editing}

1. 查找您的电子邮件，选择它并单击 **编辑草稿** 选项卡。

   ![](assets/three-281-29.jpg)

1. 单击 **电子邮件操作**，选择 **发送示例**.

   ![](assets/four.png)

1. 输入要投放的电子邮件地址，然后单击 **发送**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >触发器字段仅适用于那些利用 [电子邮件脚本](https://developers.marketo.com/documentation/velocity-script/).

## 发送基于区段的示例电子邮件 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[将分段应用于电子邮件](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. 查找您的电子邮件，选择它并单击 **编辑草稿** 选项卡。

   ![](assets/three-281-29.jpg)

1. 单击 **预览**.

   ![](assets/1.png)

1. 单击 **查看方式** 下拉框并选择 **分段**.

   ![](assets/2.png)

1. 此时会显示一个下拉列表，其中包含可用的区段。 单击该页面并选择所需的页面。

   ![](assets/3.png)

1. 使用箭头滚动浏览您的选项（在本例中，我们动态更改了主题行）。

   ![](assets/4.png)

1. 单击 **发送示例** 接收您的区段的实际测试电子邮件。

   ![](assets/5.png)

   >[!TIP]
   >
   >您还可以在电子邮件的编辑模式下根据区段发送示例电子邮件。 单击 **电子邮件操作** 下拉列表，选择 **发送示例**，然后选择您的区段。

在启动营销活动之前对内容进行采样非常重要。 量两度，剪一次！
