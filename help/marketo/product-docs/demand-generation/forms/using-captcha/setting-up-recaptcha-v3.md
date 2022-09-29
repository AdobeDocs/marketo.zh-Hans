---
description: 设置reCAPTCHA v3 - Marketo文档 — 产品文档
title: 设置reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: b848b836274d92d503e1a06cd4f7377ca57bc93e
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# 设置reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3是一种无摩擦的体验，它根据提交内容的可疑程度来对其进行评分，而无需使用文本、图像或按钮挑战。 [了解更多](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target=&quot;_blank&quot;}。

## 检索您的数据中心ID和Munchkin ID {#retrieve-your-data-center-and-munchkin-id}

对于下面“初始reCAPTCHA v3”设置部分中的步骤6，您将需要Marketo Engage订阅的数据中心ID和Munchkin ID。 这是如何找到它们。

1. 在Marketo中，单击 **管理员**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 单击 **我的帐户**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 向下滚动到支持信息。

   ![](assets/setting-up-recaptcha-v3-3.png)

## 初始reCAPTCHA v3设置 {#initial-recaptcha-v3-setup}

在Marketo之外，将执行以下步骤。

1. 转到 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;}并单击v3Admin Console。

1. 使用Google帐户登录/注册。

1. 单击创建按钮（+号）以创建新键。

1. 创建标签以标识要用于Marketo Engage的键。

1. 选择类型 **reCAPTCHA v3**. Marketo Engage当前不支持reCAPTCHA v2。

1. 添加Marketo Engage订阅使用的每个域。 未在此处设置的域将在启用reCAPTCHA的表单中返回错误。 请记住，将“datacenter”和“munchkinID”替换为 [订阅中的数据](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * 在订阅中配置的任何登陆页面域和别名

   >[!NOTE]
   >
   >例如，如果您帐户的数据中心为“sjst”，则您的允许列表域将为 `app-sjst.marketo.com`. 如果您的Munchkin ID是123-ABC-789，则您允许列表将的域将为 `123-ABC-789.mktoweb.com`.

1. 设置应接收有关此服务的任何警报的所有者和其他电子邮件地址。

1. 接受reCAPTCHA服务条款。

1. 单击 **提交**.

   >[!NOTE]
   >
   >将站点密钥和密钥保留在便于Marketo Engage配置的位置。

## 在Marketo Engage中设置CAPTCHA {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>在您执行这些步骤和 [在您的第一个Marketo表单中启用CAPTCHA](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target=&quot;_blank&quot;}，请务必立即测试表单，因为reCAPTCHA设置中的任何错误配置都可能破坏表单。

1. 在Marketo中，单击 **管理员**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 选择 **验证码** 在树上。

   ![](assets/setting-up-recaptcha-v3-5.png)

1. 单击 **编辑** 在验证码设置中。

   ![](assets/setting-up-recaptcha-v3-6.png)

1. 单击“CAPTCHA”下拉列表，然后选择reCAPTCHA v3。

   ![](assets/setting-up-recaptcha-v3-7.png)

1. 插入密钥和站点密钥。 单击 **保存** 完成时。

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[在Marketo Forms中启用CAPTCHA](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
