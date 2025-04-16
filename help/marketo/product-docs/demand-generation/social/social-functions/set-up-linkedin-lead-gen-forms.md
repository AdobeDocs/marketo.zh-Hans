---
unique-page-id: 12976798
description: 设置LinkedIn潜在客户Gen Forms - Marketo文档 — 产品文档
title: 设置LinkedIn潜在客户Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 7a8f5146126d6e8a4902be9337eef4d51e108cf0
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 设置LinkedIn潜在客户Forms {#set-up-linkedin-lead-gen-forms}

使用LinkedIn潜在客户Gen Forms在LinkedIn中运行广告营销活动并为Marketo生成潜在客户。

>[!IMPORTANT]
>
>LinkedIn正在升级由Marketo Engage LinkedIn集成使用的营销API。 在2024年6月7日至12月15日之间，这些更改将要求对您的&#x200B;**管理员** > **LaunchPoint**&#x200B;菜单中的所有LinkedIn LaunchPoint服务进行重新身份验证，以避免服务中断。 有关详细信息，请参阅[迁移常见问题解答](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>如果LinkedIn潜在客户与Marketo中的现有人员记录匹配，并且该人员记录与使用公司API创建的公司记录相关联，并且Marketo订阅未连接到CRM，则该潜在客户将不会进入Marketo Engage。

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域。

   ![](assets/set-up-linkedin-lead-gen-forms-1.png)

1. 转到&#x200B;**[!UICONTROL LaunchPoint]**，单击&#x200B;**[!UICONTROL New]**&#x200B;并选择&#x200B;**[!UICONTROL New Service]**。

   ![](assets/set-up-linkedin-lead-gen-forms-2.png)

1. 输入服务的&#x200B;_显示名称_，从下拉列表中选择&#x200B;**[!UICONTROL LinkedIn Lead Gen]**&#x200B;服务，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/set-up-linkedin-lead-gen-forms-3.png)

1. Marketo在同一浏览器中打开一个新标签页，以访问[linkedin.com](https://www.linkedin.com){target="_blank"}。 使用要用于集成的帐户登录LinkedIn。

   >[!NOTE]
   >
   >LinkedIn帐户需要访问您为其创建赞助活动的所有LinkedIn商业帐户。

   ![](assets/set-up-linkedin-lead-gen-forms-4.png)

1. 登录LinkedIn后，返回Marketo并单击&#x200B;**[!UICONTROL Authorize]**。

   ![](assets/set-up-linkedin-lead-gen-forms-5.png)

1. 出现提示时，单击&#x200B;**[!UICONTROL Allow]**&#x200B;接受Marketo应用程序安装到LinkedIn中。

   ![](assets/set-up-linkedin-lead-gen-forms-6.png)

1. 您会发现您现在已获得授权。 单击 **[!UICONTROL Next]**。

   ![](assets/set-up-linkedin-lead-gen-forms-7.png)

   >[!CAUTION]
   >
   >该服务在获得授权后一年自动过期。 要重新获得访问权限，只需单击&#x200B;**[!UICONTROL Re-Authorize]**。 根据您的浏览器设置，您可能需要重新输入LinkedIn密码。

1. 选择希望LinkedIn潜在客户能够从中进入Marketo的帐户，然后单击&#x200B;**[!UICONTROL Next]**。

   >[!TIP]
   >
   >如果您看不到所需的业务帐户，请确保已授权的用户的LinkedIn帐户对LinkedIn中的业务帐户具有“潜在客户一般表单管理器”权限。

   ![](assets/set-up-linkedin-lead-gen-forms-8.png)

1. 要接受默认的LinkedIn到Marketo字段映射，只需单击&#x200B;**[!UICONTROL Create]**&#x200B;即可。 如果要更改默认字段映射、删除字段映射或添加新字段映射，可以通过以下模式基于每个字段执行此操作。

   >[!CAUTION]
   >
   >Marketo支持将两个LinkedIn字段映射到单个Marketo字段&#x200B;_，但仅当_&#x200B;两个LinkedIn字段不在同一表单上时。 如果将同一LinkedIn表单中的两个字段映射到单个Marketo字段，则用户可能无法输入Marketo数据库。

   ![](assets/set-up-linkedin-lead-gen-forms-9.png)

   >[!NOTE]
   >
   >只有已保存到LinkedIn营销活动管理器中[表单模板](https://www.linkedin.com/help/lms/answer/79634){target="_blank"}的LinkedIn字段才会显示为LinkedIn字段，这些字段可以映射到Marketo字段。

   ![](assets/set-up-linkedin-lead-gen-forms-10.png)

做得好！ 当您在LinkedIn端成功运行营销活动时，提交LinkedIn潜在客户群表单的人员将开始流入Marketo。

>[!NOTE]
>
>您只能授权单个LinkedIn用户帐户。 如果您有多个要链接到Marketo的业务帐户，请确保该用户获得授权的LinkedIn帐户对LinkedIn中的业务帐户具有“潜在客户一般表单管理器”权限。

>[!MORELIKETHIS]
>
>[在Smart Campaign中使用LinkedIn Lead Gen表单过滤器和触发器](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
