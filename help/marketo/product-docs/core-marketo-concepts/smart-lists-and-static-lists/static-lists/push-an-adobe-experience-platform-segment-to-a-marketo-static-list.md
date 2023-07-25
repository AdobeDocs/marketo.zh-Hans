---
description: 将Adobe Experience Platform区段推送到Marketo静态列表 — Marketo文档 — 产品文档
title: 将Adobe Experience Platform区段推送到Marketo静态列表
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 将Adobe Experience Platform区段推送到Marketo静态列表 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能允许您以静态列表的形式将Adobe Experience Platform中的区段推送到Marketo。

>[!PREREQUISITES]
>
>* [编辑API角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) 以确保它具有 **读写人员** 权限（可在“访问API”下拉菜单下找到）。
>* [创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo中。
>* 转到 **管理员** > **启动点**. 查找刚刚创建的角色的名称，然后单击 **查看详细信息**. 复制信息并将其保存在 **客户端ID** 和 **客户端密码**，因为在第7步中可能需要它。
>* 在Marketo中，创建一个静态列表，或查找并选择已创建的列表。 你需要它的身份证。

1. 登录 [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 单击网格图标并选择 **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左侧导航中，单击 **目标**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 单击 **目录**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 找到Marketo Engage拼贴，然后单击 **激活**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 单击 **配置新目标**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在帐户类型下，选择现有帐户或新帐户单选按钮(在本例中，我们将选择 **现有帐户**)。 单击选择帐户图标。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果选择新帐户，您可以通过转到 **管理员** > **Munchkin** (登录后，它也是您的Marketo URL的一部分)。 您应具有的客户端ID/密码应遵循本文顶部的先决条件。

1. 选择目标帐户并单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 输入目标 **名称** 和可选描述。 单击人员创建下拉列表，然后选择“匹配现有Marketo人员并在Marketo中创建缺失的人员” _或_ “仅匹配现有Marketo人员”（在本例中，我们选择了前者）。 您还必须选择 **工作区**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果您选择“仅匹配现有Marketo人员”，则只需映射电子邮件和/或ECID，因此您可以跳过步骤13至16。

1. 此部分为可选。 单击 **创建** 跳过。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 选择您创建的目标并单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 选择要发送到Marketo的区段，然后单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果选择多个区段，则必须在“区段计划”选项卡中将每个区段映射到指定的静态列表。

   >[!IMPORTANT]
   >
   >首次将区段激活到Marketo目标后，可能需要回填在Marketo目标激活之前区段中已存在的用户档案 **长达24小时**. 今后，每当将用户档案添加到区段时，都会立即将其添加到Marketo。

1. 单击 **添加新映射**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 选择所需的属性并单击 **选择**. 在本例中，我们将选择名字、姓氏和电子邮件地址。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >您可以将属性从Experience Platform映射到Marketo Engage中您的组织有权访问的任何属性。 使用 [描述API请求](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target="_blank"} 以检索您的组织有权访问的属性字段。

1. 通过单击映射姓氏和公司名称 **添加新映射** 再次重复步骤15两次，选择 **姓氏** 然后 **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 现在该映射电子邮件地址了。 单击 **添加新映射** 再来一次。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 单击选择身份命名空间单选按钮，选择  **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >从映射电子邮件和/或ECID **身份命名空间** 制表符是确保人员在Marketo中匹配的最重要操作。 映射电子邮件将确保最高的匹配率。

1. 现在该选择源字段了。 对于电子邮件，单击光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 单击选择身份命名空间单选按钮，查找并选择 **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 要选择“公司名称”源字段，请单击其行中的光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保持选中选择属性单选按钮。 搜索“company”并选择 **companyName**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 通过单击每个源字段的光标图标并重复执行两次步骤23，选择 **姓氏** 然后 **名字**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 查看更改并单击 **完成**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
