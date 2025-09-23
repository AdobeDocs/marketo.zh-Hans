---
unique-page-id: 2360297
description: 基于IP限制Marketo登录 — Marketo文档 — 产品文档
title: 根据 IP 限制 Marketo 登录
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 11%

---

# 根据 IP 限制 Marketo 登录 {#restrict-marketo-logins-based-on-ip}

您可以根据用户的IP地址限制或允许用户访问Marketo。 操作方法如下：

>[!NOTE]
>
>**需要管理员权限**

>[!IMPORTANT]
>
>本文中的信息适用于直接在login.marketo.com登录的用户，不适用于使用Adobe ID进行身份验证的用户。 目前无法对单点登录(SSO)登录实施IP限制。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. 单击 **[!UICONTROL Login Settings]**。

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. 单击 **[!UICONTROL Edit IP Restrictions]**。

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. 选择您要&#x200B;**允许**&#x200B;还是&#x200B;**阻止**&#x200B;特定地址，请输入地址，然后单击&#x200B;**[!UICONTROL Save]**。

   >[!NOTE]
   >
   >**定义**
   >
   >* **[!UICONTROL Allowed IP addresses]**：添加允许的IP地址具有包含性。 它将包含指定的所有IP地址，并排除其他所有地址。
   >* **[!UICONTROL Block IP addresses]**：阻止特定IP访问Marketo。
   >* **[!UICONTROL Disable IP Restrictions]**：选中此项将停止任何/所有限制规则的工作。 将其用于测试目的。

   >[!NOTE]
   >
   >您可以添加多个限制，但只能全部允许或全部阻止。 不能混合和匹配允许和阻止。

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   做得不错，您的营销数据现在比以往任何时候都更安全！
