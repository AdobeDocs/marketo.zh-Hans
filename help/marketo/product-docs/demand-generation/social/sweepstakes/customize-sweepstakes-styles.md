---
unique-page-id: 2359807
description: 自定义抽奖样式 — Marketo文档 — 产品文档
title: 自定义抽奖样式
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 1%

---

# 自定义抽奖样式 {#customize-sweepstakes-styles}

当您[创建抽奖活动](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)时，您可以自定义它在登陆页面上的外观。

>[!IMPORTANT]
>
>2024年7月31日，我们开始了弃用此功能的过程。 无法再创建新资产。 现有资产将继续使用到2025年1月31日。 [了解详情](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>并非所有Marketo Engage用户都已购买此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

1. 转到&#x200B;**营销活动**。

![](assets/login-marketing-activities-1.png)

1. 选择抽奖活动，然后单击&#x200B;**编辑草稿**。

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 在抽奖编辑器中，转到&#x200B;**应用程序设置** > **外观**。

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 编辑注册按钮和进度链接的文本。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. 对于要自定义的每个元素，输入自定义CSS属性。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   **Enter按钮**的CSS示例：
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   **Enter按钮**的示例图像：
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >如果您使用带有文本的图像，请记得从上面“文本”下的&#x200B;**输入按钮**&#x200B;字段中删除文本。

1. 每次进行更改时，结果都会显示在“查看和编辑”预览中。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >在多种不同的浏览器（包括旧版本）中测试您的按钮。

   >[!MORELIKETHIS]
   >
   >下一步是向您的抽奖活动添加[注册和履行电子邮件](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md)。
