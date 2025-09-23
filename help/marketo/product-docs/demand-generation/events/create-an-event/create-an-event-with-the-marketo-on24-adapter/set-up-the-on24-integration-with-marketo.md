---
description: 设置ON24与Marketo的集成 — Marketo文档 — 产品文档
title: 设置 ON24 与 Marketo 的集成
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 8%

---

# 设置 ON24 与 Marketo 的集成{#set-up-the-on24-integration-with-marketo}

下面是如何设置您的ON24事件集成。

## 创建仅API角色 {#create-an-api-only-role}

1. 在“我的Marketo”中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. 在[!UICONTROL Security]下，单击&#x200B;**[!UICONTROL Users & Roles]**。

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. 单击&#x200B;**[!UICONTROL Roles]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL New Role]**。

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. 输入[!UICONTROL Role Name]。 打开&#x200B;**[!UICONTROL Access API]**&#x200B;菜单并选择“[!UICONTROL Read-Write Custom Object]”和“[!UICONTROL Read-Write Person]”。 单击 **[!UICONTROL Create]**。

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## 创建新用户 {#create-a-new-user}

1. 仍然在[!UICONTROL Users & Roles]中，单击&#x200B;**[!UICONTROL Users]**&#x200B;选项卡并单击&#x200B;**[!UICONTROL Invite New User]**。

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. 输入新用户的信息并单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. 选择您刚刚创建的[!UICONTROL ON24 API Only Role (all workspaces)]。 选中&#x200B;**[!UICONTROL API Only]**&#x200B;复选框。 单击 **[!UICONTROL Next]**。

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. 单击 **[!UICONTROL Send]**。

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>仅API用户不需要邀请。

## 设置ON24连接 {#set-up-on24-connection}

1. 仍在[!UICONTROL Admin]部分中，单击&#x200B;**[!UICONTROL LaunchPoint]**。

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. 单击&#x200B;**[!UICONTROL New]**，然后单击&#x200B;**[!UICONTROL New Service]**。

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. 选择[!UICONTROL display name]。 单击&#x200B;**[!UICONTROL Service]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Custom]**。 输入[!UICONTROL description]。 单击[!UICONTROL API Only User]下拉列表，然后选择在上述步骤[中创建](#create-a-new-user)的用户。 单击 **[!UICONTROL Create]**。

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. 查找您刚刚创建的自定义[!DNL LaunchPoint]服务，然后单击[!UICONTROL View Details]。

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. 突出显示、右键单击、复制并保存[!UICONTROL Client ID]（稍后您将需要它）。 重复[!UICONTROL Client Secret]。

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. 在左侧的树中，单击&#x200B;**[!UICONTROL Web Services]**。

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. 在“[!UICONTROL REST API]”下，高亮显示，右键单击，复制并保存[!UICONTROL Identity]的第一部分（直到.com中的“m”）。

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. 使用保存的客户端ID、客户端密钥和身份，导航到您的ON24帐户。 其余步骤均在此处执行，可在[ON24文档](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}中找到。
