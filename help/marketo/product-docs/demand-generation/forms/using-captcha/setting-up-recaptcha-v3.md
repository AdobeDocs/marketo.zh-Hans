---
description: 设置reCAPTCHA v3 - Marketo文档 — 产品文档
title: 设置 reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# 设置[!UICONTROL reCAPTCHA v3] {#setting-up-recaptcha-v3}

ReCAPTCHA v3是一款流畅的体验，它根据表单提交的可疑程度为其打分，而不使用文本、图像或按钮挑战。 [了解详情](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}。

## 检索您的[!UICONTROL Data Center]和[!UICONTROL Munchkin ID] {#retrieve-your-data-center-and-munchkin-id}

对于下面的初始[!UICONTROL reCAPTCHA v3]设置部分中的步骤6，您将需要Marketo Engage订阅的[!UICONTROL Data Center]和[!UICONTROL Munchkin ID]。 下面是如何找到他们的。

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 单击 **[!UICONTROL My Account]**。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 向下滚动到[!UICONTROL Support Information]。

   ![](assets/setting-up-recaptcha-v3-3.png)

## 初始[!UICONTROL reCAPTCHA v3]设置 {#initial-recaptcha-v3-setup}

在Marketo之外执行以下步骤。

1. 转到[https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"}并单击v3 Admin Console。

1. 使用Google帐户登录/注册。

1. 单击[!UICONTROL Create]按钮（+号）以创建新密钥。

1. 创建标签以标识要用于Marketo Engage的键。

1. 选择类型&#x200B;**[!UICONTROL reCAPTCHA v3]**。 Marketo Engage当前不支持reCAPTCHA v2。

1. 添加Marketo Engage订阅使用的每个域。 此处未设置的域将在启用reCAPTCHA的表单中返回错误。 请记得将单词“datacenter”和“munchkinID”替换为订阅[中的](#retrieve-your-data-center-and-munchkin-id)数据。

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * 订阅中配置的任何登陆页面域和别名

   >[!NOTE]
   >
   >例如，如果帐户的[!UICONTROL Data Center]为“sjst”，则允许列表的域将为`app-sjst.marketo.com`。 如果[!UICONTROL Munchkin ID]是123-ABC-789，则允许列表的域将为`123-ABC-789.mktoweb.com`。

1. 设置所有者和应接收有关此服务的所有警报的其他电子邮件地址。

1. 接受reCAPTCHA服务条款。

1. 单击 **[!UICONTROL Submit]**。

   >[!NOTE]
   >
   >为Marketo Engage配置随时准备站点密钥和密钥。

## 在Marketo Engage中设置验证码 {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>按照这些步骤操作并[在第一个Marketo表单](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}中启用验证码后，请务必立即测试表单，因为reCAPTCHA设置中的任何错误配置都会破坏表单。

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 在树中选择&#x200B;**[!UICONTROL CAPTCHA]**。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. 单击&#x200B;**[!UICONTROL Edit]**&#x200B;设置上的[!UICONTROL CAPTCHA]。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. 单击[!UICONTROL CAPTCHA]下拉菜单并选择[!UICONTROL reCAPTCHA v3]。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. 插入&#x200B;**[!UICONTROL Secret Key]**&#x200B;和&#x200B;**[!UICONTROL Site Key]**。 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[在Marketo Forms中启用验证码](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
