---
description: 将Adobe Experience Platform区段推送到Marketo静态列表 — Marketo文档 — 产品文档
title: 将Adobe Experience Platform区段推送到Marketo静态列表
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: ccc62b22f260293ac193ce03a31e4f03aba34768
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 将Adobe Experience Platform区段推送到Marketo静态列表 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能允许您以静态列表的形式将位于Adobe Experience Platform中的区段推送到Marketo。

>[!PREREQUISITES]
>
>* [编辑API角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) 确保它有 **读写人员** 权限（位于访问API下拉列表下）。
>* [创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 转到 **管理员** > **Launchpoint**. 查找您刚刚创建的角色的名称，然后单击 **查看详细信息**. 复制信息并将其保存在 **客户端ID** 和 **客户端密钥**，因为在步骤7中，您可能需要它。
>* 在Marketo中，创建静态列表，或查找并选择一个已创建的列表。 你需要它的身份证。


1. 登录到 [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 单击网格图标，然后选择 **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左侧导航栏中，单击 **目标**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 单击 **目录**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 查找Marketo Engage拼贴并单击 **激活**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 单击 **配置新目标**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在“帐户类型”下，选择“现有帐户”或“新建帐户”单选按钮(在本例中，我们选择 **现有帐户**)。 单击选择帐户图标。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果您选择“新帐户”，则可以通过以下路径找到您的Munchkin ID: **管理员** > **蒙奇金** (登录后，它也会成为Marketo URL的一部分)。 客户端ID/密钥您应当具有，以便遵循本文顶部的先决条件。

1. 选择目标帐户并单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 输入目标 **名称** 和可选描述。 单击“人员创建”下拉列表，然后选择“在Marketo中匹配现有的Marketo人员并创建缺失的人员” _或_ “仅匹配现有Marketo人员”（在此示例中，我们选择前者）。 您还必须选择 **工作区**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果您选择“仅匹配现有Marketo人员”，则只需映射电子邮件和/或ECID，即可跳过步骤13-16。

1. 此部分是可选的。 单击 **创建** 跳过。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 选择您创建的目标并单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 选择要发送到Marketo的区段，然后单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果选择多个区段，则必须在区段计划选项卡中将每个区段映射到指定的静态列表。

   >[!IMPORTANT]
   >
   >首次将区段激活到Marketo目标后，可能需要在Marketo目标激活之前回填区段中已存在的用户档案 **长达24小时**. 今后，每当将用户档案添加到区段时，他们都会立即添加到Marketo。

1. 单击 **添加新映射**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 选择所需的属性并单击 **选择**. 在本例中，我们选择的是名字、姓氏和电子邮件地址。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >您可以将属性从Experience Platform映射到贵组织在Marketo Engage中有权访问的任何属性。 使用 [描述API请求](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target=&quot;_blank&quot;}以检索贵组织有权访问的属性字段。

1. 通过单击 **添加新映射** 重复步骤15，选择 **lastName** 然后 **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 现在该映射电子邮件地址了。 单击 **添加新映射** 再次。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 单击“选择身份命名空间”单选按钮，然后选择  **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >从映射电子邮件和/或ECID **身份命名空间** 选项卡是确保人员在Marketo中进行匹配时最重要的操作。 映射电子邮件将确保最高匹配率。

1. 现在该选择源字段了。 对于电子邮件，单击光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 单击“选择身份命名空间”单选按钮，找到并选择 **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 要选择公司名称源字段，请单击其行中的光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保持选中选择属性单选按钮。 搜索“company”并选择 **companyName**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 通过单击每个的光标图标并重复步骤23两次来映射姓氏和名字的源字段，选择 **lastName** 然后 **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 查看更改并单击 **完成**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
