---
description: 如何自定义登陆页面域的HTTP标头，包括严格传输安全和X-Frame-Options。
title: 登陆页面标头
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: 'https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 5%
---
# 登陆页面标头 {#landing-page-headers}

请按照以下步骤自定义登陆页面域上的某些HTTP标头。

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/landing-page-headers-1.png)

1. 单击 **[!UICONTROL Landing Pages]**。

   ![](assets/landing-page-headers-2.png)

1. 单击登陆页面HTTP标头旁边的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/landing-page-headers-3.png)

1. 选择所需的设置，完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>使用此项可保证始终通过HTTPS提供到登陆页面的连接（应仅针对登陆页面受SSL保护的订阅进行设置）</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>允许您定义是否可以在外部网页中嵌入Marketo Engage托管的资源</td>
 </tr>
</table>

>[!CAUTION]
>
>务必与IT团队一起查看这些设置，以确定应将组织的策略设置为什么内容。 不正确的设置可能会阻止某些访客访问您的登陆页面。
