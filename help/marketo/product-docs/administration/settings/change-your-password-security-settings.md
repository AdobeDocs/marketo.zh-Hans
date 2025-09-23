---
unique-page-id: 2360185
description: 更改密码安全设置 — Marketo文档 — 产品文档
title: 更改密码安全设置
exl-id: cda7ec70-32aa-4e0a-86b2-eb9bea70ef72
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 11%

---

# 更改密码安全设置 {#change-your-password-security-settings}

控制订阅的密码策略。 操作方法如下：

>[!NOTE]
>
>**需要管理员权限**

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/change-your-password-security-settings-1.png)

1. 单击 **[!UICONTROL Login Settings]**。

   ![](assets/change-your-password-security-settings-2.png)

1. 在&#x200B;**[!UICONTROL Security Settings]**&#x200B;下，单击&#x200B;**[!UICONTROL Edit]**。

   ![](assets/change-your-password-security-settings-3.png)

1. 选择&#x200B;**[!UICONTROL Template]**。 有关高级选项，请单击&#x200B;**[!UICONTROL Advanced]**&#x200B;下拉列表。

   ![](assets/change-your-password-security-settings-4.png)

   >[!NOTE]
   >
   >模板只是预建配置。 **[!UICONTROL Standard Security]**&#x200B;很好。 **[!UICONTROL High Security]**&#x200B;是最强的。 **[!UICONTROL Custom]**&#x200B;允许您自己制作。

   >[!TIP]
   >
   >在&#x200B;**[!UICONTROL Custom]**&#x200B;中，选中方框以指示用户创建密码时要包含哪些特性。

1. 设置&#x200B;**[!UICONTROL Expiration]**。 此功能自动要求用户在一定时间后重置密码。 这包括管理员用户。

   ![](assets/change-your-password-security-settings-5.png)

   >[!CAUTION]
   >
   >现有用户不会收到更改的通知。 首先将&#x200B;**[!UICONTROL Expiration]**&#x200B;设置为30天以确保所有人都已更新到新设置，然后将此设置更改回原始节奏。

1. 设置&#x200B;**[!UICONTROL Inactive Session Timeout]**。 此值确定用户在必须重新登录Marketo之前可以处于非活动状态的时长。

   ![](assets/change-your-password-security-settings-6.png)
