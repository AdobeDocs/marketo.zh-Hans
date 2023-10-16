---
unique-page-id: 2359807
description: 自定义抽奖样式 — Marketo文档 — 产品文档
title: 自定义抽奖样式
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# 自定义抽奖样式 {#customize-sweepstakes-styles}

当您 [设置抽奖活动](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，您可以自定义登陆页面上的显示方式。

>[!AVAILABILITY]
>
>并非所有Marketo Engage用户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

1. 转到 **营销活动**.

![](assets/login-marketing-activities-1.png)

1. 选择抽奖活动，然后单击 **编辑草稿**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 在“抽奖活动”编辑中，转到 **应用程序设置** > **外观**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 编辑注册按钮和进度链接的文本。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. 对于要自定义的每个元素，输入自定义CSS属性。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   示例CSS **输入按钮**：
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   示例图像 **输入按钮**：
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >如果您使用带有文本的图像，请记住从 **输入按钮** 字段。

1. 每次进行更改时，结果都会显示在“查看和编辑”预览中。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >在多种不同的浏览器（包括旧版本）中测试您的按钮。

   >[!MORELIKETHIS]
   >
   >下一步是添加 [注册和履行电子邮件通知您的抽奖活动](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
