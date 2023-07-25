---
unique-page-id: 12980661
description: 将Google客户匹配项作为LaunchPoint服务添加 — Marketo文档 — 产品文档
title: 将Google Customer Match添加为LaunchPoint Service
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 2%

---

# 将Google Customer Match添加为LaunchPoint Service {#add-google-customer-match-as-a-launchpoint-service}

通过此集成，您可以将Marketo受众发送到Google，以使用Google AdWords进行定位，以及跨YouTube、Search和Gmail重新定位受众。

>[!NOTE]
>
>**需要管理员权限**

1. 转到 **管理员**.

   ![](assets/admin.png)

1. 单击 **启动点**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. 选择 **新** 则 **新服务**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. 输入 **显示名称** 并选择 **Google客户匹配** 从 **服务** 下拉菜单。 单击&#x200B;**创建**。

   ![](assets/chooseservice.png)

1. 要连接Google AdWords帐户，请单击 **授权**.

   ![](assets/authorizeaccount-1.png)

1. Google将在新选项卡中打开。 从这里，登录到您的Google AdWords帐户。

   >[!CAUTION]
   >
   >为了使Marketo能够跨多个AdWords帐户发送受众，您执行以下步骤中授权的Google用户需要有权访问 _所有_ 这些账户的10%。

   ![](assets/chooseaccount.png)

1. 查看请求的权限，然后单击 **允许**.

   ![](assets/reviewpermissions.png)

1. 您的Google AdWords帐户现已连接到Marketo。 单击&#x200B;**创建**。

   ![](assets/authorizesuccess.png)

   太棒了！ 现在，您将在Installed Services选项卡中看到作为LaunchPoint服务列出的Google匹配受众。

>[!NOTE]
>
>Google Customer Match集成只能容纳一个经理帐户以及该经理帐户内的所有子帐户。 不支持多个管理器帐户。
