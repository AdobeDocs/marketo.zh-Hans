---
description: 设置reCAPTCHA v3 - Marketo文档 — 产品文档
title: 设置reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 设置reCAPTCHA {#setting-up-recaptcha}

简介文本

## 设置reCAPTCHA v3 {#setting-up-recaptcha-v3}

文本：描述v3 — 在Marketo Engage之外执行以下步骤。

1. 转到 [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;}并单击v3Admin Console。

1. 使用Google帐户登录/注册。

1. 单击创建（+号）按钮以创建新键。

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
>在Marketo Engage配置中，请准备好站点密钥和密钥。

## 在Marketo Engage中设置CAPTCHA {#setting-up-captcha-in-marketo-engage}

1. 在Marketo中，单击 **管理员** 选择 **验证码**.

PICC

1. 单击 **编辑** 在验证码设置中。

PICC

1. 单击“CAPTCHA”下拉列表，然后选择reCAPTCHA v3。

PICC

1. 插入密钥和站点密钥。 单击 **保存** 完成时。

PICC
