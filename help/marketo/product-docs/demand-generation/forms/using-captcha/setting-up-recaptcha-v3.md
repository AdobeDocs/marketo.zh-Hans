---
description: 设置reCAPTCHA v3 - Marketo文档 — 产品文档
title: 设置reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 24942664d613fa2851bad7a0dd3862027deacf37
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 设置reCAPTCHA v3 {#setting-up-recaptcha-v3}

简介文本

## 初始reCAPTCHA v3设置 {#initial-recaptcha-v3-setup}

文本：描述v3 — 在Marketo Engage之外执行以下步骤。

1. 转到 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;}并单击v3Admin Console。

1. 使用Google帐户登录/注册。

1. 单击创建按钮（+号）以创建新键。

1. 创建标签以标识要用于Marketo Engage的键。

1. 选择类型 **reCAPTCHA v3**. Marketo Engage当前不支持reCAPTCHA v2。

1. 添加Marketo Engage订阅使用的每个域。 未在此处设置的域将在启用reCAPTCHA的表单中返回错误。

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * 在订阅中配置的任何登陆页面域和别名

1. 设置应接收有关此服务的任何警报的所有者和其他电子邮件地址。

1. 接受reCAPTCHA服务条款。

1. 单击 **提交**.

>[!NOTE]
>
>将站点密钥和密钥保留在便于Marketo Engage配置的位置。

## 在Marketo Engage中设置CAPTCHA {#setting-up-captcha-in-marketo-engage}

1. 在Marketo中，单击 **管理员**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. 选择 **验证码** 在树上。

   ![](assets/setting-up-recaptcha-v3-2.png)

1. 单击 **编辑** 在验证码设置中。

   ![](assets/setting-up-recaptcha-v3-3.png)

1. 单击“CAPTCHA”下拉列表，然后选择reCAPTCHA v3。

   ![](assets/setting-up-recaptcha-v3-4.png)

1. 插入密钥和站点密钥。 单击 **保存** 完成时。

   ![](assets/setting-up-recaptcha-v3-5.png)
