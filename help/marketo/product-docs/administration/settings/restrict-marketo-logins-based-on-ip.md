---
unique-page-id: 2360297
description: 基于IP限制营销人员登录——营销人员文档——产品文档
title: 限制基于IP的营销人员登录
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 基于IP {#restrict-marketo-logins-based-on-ip}限制营销人员登录

您可以根据用户的IP地址限制或允许用户访问Marketo。 这是方法。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>本文中的信息仅适用于login.marketo.com上的直接登录。 目前无法对单点登录(SSO)登录强制实施IP限制。

1. 在&#x200B;**Admin**&#x200B;下，单击&#x200B;**登录设置**。

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. 单击&#x200B;**编辑IP限制**。

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. 选择是&#x200B;**允许**&#x200B;还是&#x200B;**阻止**&#x200B;特定地址，输入地址，然后单击&#x200B;**保存**。

   >[!NOTE]
   >
   >**定义**
   >
   >* **允许的IP地址**:添加允许的IP地址是包含的。它将包括指定的所有IP地址，并排除其他所有地址。
   >* **块IP地址**:阻止特定IP访问Marketo。
   >* **禁用IP限制**:选中此项将阻止任何／所有限制规则工作。用于测试目的。


   >[!NOTE]
   >
   >您可以添加多个限制，但只能将其设置为“允许”或“全部阻止”。 您不能混音和匹配允许和阻止。

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   您的营销数据做得好，现在比以往更安全！
