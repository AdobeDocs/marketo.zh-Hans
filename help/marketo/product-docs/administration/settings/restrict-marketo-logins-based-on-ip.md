---
unique-page-id: 2360297
description: 基于IP限制Marketo登录 — Marketo文档 — 产品文档
title: 基于IP限制Marketo登录
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 基于IP限制Marketo登录 {#restrict-marketo-logins-based-on-ip}

您可以根据用户的IP地址限制或允许用户访问Marketo。 具体方法如下。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>本文中的信息仅适用于login.marketo.com上的直接登录。 目前无法对单点登录(SSO)登录强制执行IP限制。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. 单击 **[!UICONTROL 登录设置]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. 单击 **[!UICONTROL 编辑IP限制]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. 选择是否要 **允许** 或 **块** 指定地址，输入地址，然后单击 **[!UICONTROL 保存]**.

   >[!NOTE]
   >
   >**条件**
   >
   >* **[!UICONTROL 允许的IP地址]**：添加允许的IP地址具有包容性。 它将包含指定的所有IP地址，并排除其他所有地址。
   >* **[!UICONTROL 阻止IP地址]**：阻止特定IP访问Marketo。
   >* **[!UICONTROL 禁用IP限制]**：选中此项将停止任何/所有限制规则的工作。 将其用于测试目的。

   >[!NOTE]
   >
   >您可以添加多个限制，但只能全部允许或全部阻止。 不能混合和匹配允许和阻止。

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   做得不错，您的营销数据现在比以往任何时候都更安全！
