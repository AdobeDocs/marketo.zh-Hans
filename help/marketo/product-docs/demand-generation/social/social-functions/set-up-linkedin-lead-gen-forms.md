---
unique-page-id: 12976798
description: 设置LinkedIn潜在客户群Forms - Marketo文档 — 产品文档
title: 设置LinkedIn潜在客户Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 设置LinkedIn潜在客户Gen Forms {#set-up-linkedin-lead-gen-forms}

使用LinkedIn潜在客户Gen Forms在LinkedIn中运行广告营销活动并为Marketo生成潜在客户。

>[!IMPORTANT]
>
>linkedIn正在升级其由Marketo EngageLinkedIn集成使用的营销API。 在2024年6月7日至12月15日之间，这些更改将需要重新验证您&#x200B;**管理员** > **LaunchPoint**&#x200B;菜单中的所有LinkedIn LaunchPoint服务，以避免服务中断。 有关详细信息，请参阅[迁移常见问题解答](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>如果LinkedIn商机与Marketo中与使用公司API创建的公司记录关联的现有人员记录匹配，并且Marketo订阅未连接到CRM，则它不会Marketo Engage。

1. 转到Marketo **管理员**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到&#x200B;**LaunchPoint**，单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建服务**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 为您的服务输入&#x200B;**显示名称**，从下拉列表中选择&#x200B;**LinkedIn Lead Gen**&#x200B;服务，然后单击&#x200B;**下一步**。

   ![](assets/linkedin-lead-gen.png)

1. Marketo在同一浏览器中打开一个新标签页，以访问[linkedin.com](https://www.linkedin.com)。 使用要用于集成的帐户登录LinkedIn。

   >[!NOTE]
   >
   >linkedIn帐户需要访问您为其创建赞助营销活动的所有LinkedIn业务帐户。

   ![](assets/linkedin-login.png)

1. 登录LinkedIn后，返回Marketo并单击&#x200B;**授权**。

   ![](assets/linkedin-lead-gen-authorize.png)

1. 出现提示时，单击&#x200B;**允许**&#x200B;接受Marketo应用程序安装到LinkedIn中。

   ![](assets/linkedin-marketo-allow.png)

1. 您会发现您现在已获得授权。 单击&#x200B;**下一步**。

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >该服务在获得授权后一年自动过期。 要重新获得访问权限，只需单击&#x200B;**重新授权**。 根据浏览器设置，您可能需要重新输入LinkedIn密码。

1. 选择要让LinkedIn潜在客户进入Marketo的帐户，然后单击&#x200B;**下一步**。

   >[!TIP]
   >
   >如果您看不到所需的业务帐户，请确保已授权用户的LinkedIn帐户对LinkedIn中的业务帐户具有潜在客户一般表单管理员权限。

   ![](assets/linkedin-pages-to-capture.png)

1. 要接受默认的LinkedIn到Marketo字段映射，只需单击&#x200B;**创建**。 如果要更改默认字段映射、删除字段映射或添加新字段映射，可以通过以下模式基于每个字段执行此操作。

   >[!CAUTION]
   >
   >Marketo支持将两个LinkedIn字段映射到一个Marketo字段&#x200B;**，但仅当**&#x200B;两个LinkedIn字段不在同一表单上时。 如果将同一LinkedIn表单中的两个字段映射到单个Marketo字段，则用户可能无法输入Marketo数据库。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >只有已保存到LinkedIn Campaign Manager中的[表单模板](https://www.linkedin.com/help/lms/answer/79634)的LinkedIn字段才会显示为“可映射到Marketo字段的LinkedIn字段”。

   ![](assets/linkedin-installed-services.png)

做得好！ 当您在LinkedIn端成功开展营销活动时，提交LinkedIn潜在客户群表单的人员将开始流入Marketo。

>[!NOTE]
>
>您只能授权一个LinkedIn用户帐户。 如果您有多个要链接到Marketo的业务帐户，请确保该用户获得授权的LinkedIn帐户对LinkedIn中的业务帐户具有“潜在客户一般表单管理器”权限。

>[!MORELIKETHIS]
>
>[在Smart Campaign中使用LinkedIn Lead Gen表单过滤器和触发器](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
