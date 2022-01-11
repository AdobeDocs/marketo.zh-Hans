---
description: 登陆页面标题 — Marketo文档 — 产品文档
title: 登陆页面标题
hide: true
hidefromtoc: true
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
source-git-commit: 7950fb6ef4a0f653b3125ec381c652056bd47327
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# 登陆页面标题 {#landing-page-headers}

请按照以下步骤自定义登陆页面域上的某些HTTP标头。

1. 在Marketo中，单击 **管理员**.

   ![](assets/landing-page-headers-1.png)

1. 单击 **登陆页面**.

   ![](assets/landing-page-headers-2.png)

1. 单击 **编辑** 登陆页面HTTP头旁边的。

   ![](assets/landing-page-headers-3.png)

1. 选择所需的设置并单击 **保存** 完成时。

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>严格传输安全</strong></td>
  <td>使用此选项可确保始终通过HTTPS提供与登陆页面的连接（只应为使用SSL保护的登陆页面的订阅设置）</td>
 </tr>
 <tr>
  <td><strong>X-Frame-Options</strong></td>
  <td>允许您定义是否可以将托管的Marketo Engage资产嵌入到外部网页中</td>
 </tr>
</table>

>[!CAUTION]
>
>请与您的IT团队一起查看这些设置，以确定贵组织的策略应设置为什么，这一点非常重要。 错误设置可能会阻止某些访客访问您的登陆页面。
