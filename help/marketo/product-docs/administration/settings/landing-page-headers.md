---
description: 登陆页标题 — Marketo文档 — 产品文档
title: 登陆页标题
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---

# 登陆页标题 {#landing-page-headers}

请按照以下步骤自定义登陆页面域上的某些HTTP标头。

1. 在Marketo中，单击 **[!UICONTROL 管理员]**.

   ![](assets/landing-page-headers-1.png)

1. 单击 **[!UICONTROL 登陆页面]**.

   ![](assets/landing-page-headers-2.png)

1. 单击 **[!UICONTROL 编辑]** 在登陆页面HTTP标头旁边。

   ![](assets/landing-page-headers-3.png)

1. 选择所需的设置并单击 **[!UICONTROL 保存]** 完成时。

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[！UICONTROL严格传输安全]</strong></td>
  <td>使用此选项可保证始终通过HTTPS提供到登陆页面的连接（应仅针对登陆页面受SSL保护的订阅进行设置）</td>
 </tr>
 <tr>
  <td><strong>[！UICONTROL X-Frame-Options]</strong></td>
  <td>用于定义是否可以在外部网页中嵌入Marketo Engage托管的资源</td>
 </tr>
</table>

>[!CAUTION]
>
>务必与IT团队一起查看这些设置，以确定贵组织的策略应设置为什么。 不正确的设置可能会阻止某些访客访问您的登陆页面。
