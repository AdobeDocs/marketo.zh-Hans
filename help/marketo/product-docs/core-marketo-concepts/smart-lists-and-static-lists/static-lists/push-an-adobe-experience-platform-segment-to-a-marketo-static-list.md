---
description: 将Adobe Experience Platform区段推送到Marketo静态列表 — Marketo文档 — 产品文档
title: 将Adobe Experience Platform区段推送到Marketo静态列表
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# 将Adobe Experience Platform区段推送到Marketo静态列表 {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

此功能允许您以静态列表的形式将Adobe Experience Platform中的区段推送到Marketo Engage。

>[!PREREQUISITES]
>
>* [编辑API角色](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role){target="_blank"}以确保它具有&#x200B;**读写人员**&#x200B;权限（可在“访问API”下拉列表中找到）。
>* 在Marketo中[创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}。
>* 转到&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Launchpoint]**。 查找您刚刚创建的角色的名称，然后单击&#x200B;**[!UICONTROL View Details]**。 复制并保存&#x200B;**[!UICONTROL Client ID]**&#x200B;和&#x200B;**[!UICONTROL Client Secret]**&#x200B;中的信息，因为在第7步中可能需要它。
>* 在Marketo中，创建一个静态列表，或查找并选择已创建的列表。 你需要它的身份证。

1. 登录到[Adobe Experience Platform](https://experience.adobe.com/){target="_blank"}。

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 单击网格图标并选择&#x200B;**[!UICONTROL Experience Platform]**。

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左侧导航中，单击&#x200B;**[!UICONTROL Destinations]**。

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 单击 **[!UICONTROL Catalog]**。

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 找到Marketo Engage拼贴，然后单击&#x200B;**[!UICONTROL Activate]**。

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 单击 **[!UICONTROL Configure New Destination]**。

   ![](assets/push-an-adobe-experience-platform-segment-6.png)

1. 在“帐户类型”下，选择“现有帐户”或“新帐户”单选按钮（在本例中，我们将选择&#x200B;**[!UICONTROL Existing Account]**）。 单击选择帐户图标。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果选择新帐户，您可以通过转到&#x200B;**[!UICONTROL Admin]** > **[!UICONTROL Munchkin]**&#x200B;来查找您的Munchkin ID(登录后，它也是您的Marketo URL的一部分)。 您应该具有的客户端ID/密钥，应遵循本文顶部的先决条件。

1. 选择目标帐户并单击&#x200B;**[!UICONTROL Select]**。

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 输入目标&#x200B;**[!UICONTROL Name]**&#x200B;和可选描述。 单击人员创建下拉列表，然后选择“在Marketo中匹配现有Marketo人员并创建缺少的人员”_或_“仅匹配现有Marketo人员”（在本例中，我们选择了前者）。 您还必须选择一个&#x200B;**[!UICONTROL Workspace]**。

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果您选择“[!UICONTROL Match Existing Marketo People Only]”，则只需映射电子邮件和/或ECID，因此您可以跳过步骤13至16。

1. 此部分为可选部分。 单击&#x200B;**[!UICONTROL Create]**&#x200B;跳过。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 选择您创建的目标，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 选择要发送到Marketo的区段，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果选择多个区段，则必须将每个区段映射到[!UICONTROL Segment Schedule]选项卡中的指定静态列表。

   >[!IMPORTANT]
   >
   >首次将区段激活到Marketo目标后，回填在Marketo目标激活之前区段中已存在的配置文件可能需要&#x200B;_长达24小时_。 今后，无论用户档案何时添加到区段，都会立即将其添加到Marketo。

1. 单击 **[!UICONTROL Add New Mapping]**。

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 选择所需的属性，然后单击&#x200B;**[!UICONTROL Select]**。 在本例中，我们将选择名字、姓氏和电子邮件地址。

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >您可以将属性从Experience Platform映射到您的组织在Marketo Engage中有权访问的任何属性。 使用[Describe API请求](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database#describe){target="_blank"}检索您的组织有权访问的属性字段。

1. 通过再次单击&#x200B;**[!UICONTROL Add New Mapping]**&#x200B;并重复步骤15两次，依次选择&#x200B;**[!UICONTROL lastName]**&#x200B;和&#x200B;**[!UICONTROL companyName]**&#x200B;来映射姓氏和公司名称。

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 现在该映射电子邮件地址了。 再次单击&#x200B;**[!UICONTROL Add New Mapping]**。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 单击“选择身份命名空间”单选按钮，选择&#x200B;**[!UICONTROL Email]**，然后单击&#x200B;**[!UICONTROL Select]**。

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >从&#x200B;**[!UICONTROL Identity Namespace]**&#x200B;选项卡映射电子邮件和/或ECID是确保人员在Marketo中匹配的最重要操作。 映射电子邮件将确保最高的匹配率。

1. 现在该选择源字段了。 对于电子邮件，单击光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 单击“选择身份命名空间”单选按钮，查找并选择&#x200B;**[!UICONTROL Email]**，然后单击&#x200B;**[!UICONTROL Select]**。

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 要选择“公司名称”来源字段，请单击该行中的光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保持选中选择属性单选按钮。 搜索“公司”并选择&#x200B;**[!UICONTROL companyName]**，然后单击&#x200B;**[!UICONTROL Select]**。

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 通过单击每个的光标图标并重复第23步两次，选择&#x200B;**[!UICONTROL lastName]**，然后选择&#x200B;**[!UICONTROL firstName]**&#x200B;来映射“姓氏”和“名字”的源字段。

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 查看更改并单击&#x200B;**[!UICONTROL Finish]**。

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
