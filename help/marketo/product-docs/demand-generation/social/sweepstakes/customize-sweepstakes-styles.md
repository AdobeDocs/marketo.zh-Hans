---
unique-page-id: 2359807
description: 自定义抽奖样式 — Marketo文档 — 产品文档
title: 自定义抽奖样式
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# 自定义抽奖样式 {#customize-sweepstakes-styles}

当您 [创建抽奖](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)，则可以自定义其在登陆页面上的外观。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的销售代表。

1. 转到 **营销活动**.

![](assets/login-marketing-activities-1.png)

1. 选择抽奖，然后单击 **编辑草稿**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 在抽奖活动编辑中，转到 **应用程序设置** > **外观**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 编辑注册按钮和进度链接的文本。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. 对于要自定义的每个元素，输入自定义CSS属性。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   示例CSS **输入按钮**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   示例图像 **输入按钮**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >如果您使用的图像上带有文本，请记得从 **输入按钮** 字段。

1. 进行每次更改时，结果都会显示在“查看和编辑”预览中。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >在多个不同的浏览器中测试您的按钮，包括旧版本。

   >[!MORELIKETHIS]
   >
   >下一步是添加 [向您的抽奖活动注册和履行电子邮件](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
