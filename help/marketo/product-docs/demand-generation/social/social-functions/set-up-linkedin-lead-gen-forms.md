---
unique-page-id: 12976798
description: 设置LinkedIn潜在客户代Forms- Marketo文档——产品文档
title: 设置LinkedIn领头将Forms
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---


# 设置LinkedIn潜在客户代Forms{#set-up-linkedin-lead-gen-forms}

使用LinkedIn潜在客户代Forms在LinkedIn中运行广告活动，并为Marketo生成潜在客户。

>[!NOTE]
>
>**需要管理员权限**

1. 转到Marketo **Admin**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转至&#x200B;**LaunchPoint**，单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建服务**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 输入服务的&#x200B;**显示名称**，从下拉列表中选择&#x200B;**LinkedIn Lead Gen**&#x200B;服务，然后单击&#x200B;**Next**。

   ![](assets/linkedin-lead-gen.png)

1. Marketo在同一浏览器中打开一个指向[linkedin.com](https://www.linkedin.com)的新选项卡。 使用要用于集成的帐户登录到LinkedIn。

   >[!NOTE]
   >
   >LinkedIn帐户需要访问您正在为其创建赞助活动的所有LinkedIn业务帐户。

   ![](assets/linkedin-login.png)

1. 登录LinkedIn后，返回Marketo并单击&#x200B;**授权**。

   ![](assets/linkedin-lead-gen-authorize.png)

1. 出现提示时，单击&#x200B;**允许**&#x200B;接受Marketo应用程序安装到LinkedIn中。

   ![](assets/linkedin-marketo-allow.png)

1. 您会注意到您现在已获得授权。 单击&#x200B;**下一步**。

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >该服务在授权后一年自动过期。 要重新获得访问权，只需单击&#x200B;**重新授权**。 您可能必须重新输入LinkedIn密码，具体取决于您的浏览器设置。

1. 选择您希望LinkedIn潜在客户代从中进入Marketo的帐户，然后单击&#x200B;**下一步**。

   >[!TIP]
   >
   >如果看不到您期望的业务帐户，请确保正在授权的用户的LinkedIn帐户在LinkedIn中对业务帐户具有潜在客户生成表单管理器权限。

   ![](assets/linkedin-pages-to-capture.png)

1. 要接受默认的LinkedIn到Marketo字段映射，只需单击&#x200B;**创建**。 如果要更改默认字段映射、删除字段映射或添加新字段映射，您可以通过下面的模式逐字段执行此操作。

   >[!CAUTION]
   >
   >Marketo支持将两个LinkedIn字段映射到单个Marketo字段，**但仅当**&#x200B;两个LinkedIn字段不在同一表单时。 如果将同一LinkedIn表单中的两个字段映射到单个Marketo字段，则用户可能无法输入您的Marketo数据库。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >只有已保存到LinkedIn活动管理器中[表单模板](https://www.linkedin.com/help/lms/answer/79634)的LinkedIn字段才会显示为可映射到Marketo字段的LinkedIn字段。

   ![](assets/linkedin-installed-services.png)

干得好！ 提交LinkedIn潜在客户代表表单的人员将在LinkedIn端运行成功开始时活动流入Marketo。

>[!NOTE]
>
>您只能对单个LinkedIn用户帐户授权。 如果您有多个要链接到Marketo的业务帐户，请确保正在授权的用户的LinkedIn帐户对LinkedIn中的业务帐户具有潜在客户生成表单管理者权限。

>[!MORELIKETHIS]
>
>[在智能过滤器中使用LinkedIn潜在客户生成表单活动和触发器](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
