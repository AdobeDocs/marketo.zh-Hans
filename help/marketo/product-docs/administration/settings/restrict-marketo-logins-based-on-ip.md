---
unique-page-id: 2360297
description: 基于IP限制Marketo登录 — Marketo文档 — 产品文档
title: 基于IP限制Marketo登录
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# 基于IP限制Marketo登录 {#restrict-marketo-logins-based-on-ip}

您可以根据用户的IP地址限制或允许用户访问Marketo。 这是方法。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>本文中的信息仅适用于login.marketo.com上的直接登录。 目前无法对单点登录(SSO)登录强制实施IP限制。

1. 在 **管理员**，单击 **登录设置**.

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. 单击 **编辑IP限制**.

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. 选择是否要 **允许** 或 **块** 指定地址，输入地址，然后单击 **保存**.

   >[!NOTE]
   >
   >**条件**
   >
   >* **允许的IP地址**:添加允许的IP地址是包含性的。 它将包含指定的所有IP地址，并排除其他所有IP地址。
   >* **阻止IP地址**:阻止特定IP访问Marketo。
   >* **禁用IP限制**:选中此选项将阻止任何/所有限制规则工作。 用于测试目的。


   >[!NOTE]
   >
   >您可以添加多个限制，但只能将其设为“全部允许”或“全部阻止”。 您不能混合匹配允许的和阻止的。

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   您的营销数据做得不错，现在比以往更安全！
