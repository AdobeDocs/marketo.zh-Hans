---
unique-page-id: 12976798
description: 设置LinkedIn Lead Gen Forms - Marketo文档 — 产品文档
title: 设置LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 设置LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

使用LinkedIn潜在客户代Forms在LinkedIn中运行广告促销活动，并为Marketo生成潜在客户。

>[!NOTE]
>
>**需要管理员权限**

1. 转到Marketo **管理员**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到 **LaunchPoint**，单击 **新建** 选择 **新服务**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 输入 **显示名称** 对于您的服务，请选择 **linkedIn牵头代** 服务，然后单击 **下一个**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo会在同一浏览器中打开一个新选项卡，以 [linkedin.com](https://www.linkedin.com). 使用您要用于集成的帐户登录LinkedIn。

   >[!NOTE]
   >
   >LinkedIn帐户需要访问您为其创建赞助促销活动的所有LinkedIn业务帐户。

   ![](assets/linkedin-login.png)

1. 登录LinkedIn后，返回Marketo并单击 **授权**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. 出现提示时，单击 **允许** 接受将Marketo应用程序安装到LinkedIn中。

   ![](assets/linkedin-marketo-allow.png)

1. 你会注意到你现在有权。 单击 **下一个**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >服务在授权后一年自动过期。 要重新获得访问权，只需单击 **重新授权**. 您可能需要重新输入LinkedIn密码，具体取决于您的浏览器设置。

1. 选择您希望LinkedIn潜在客户代从进入Marketo的帐户并单击 **下一个**.

   >[!TIP]
   >
   >如果您没有看到您期望的业务帐户，请确保正在授权的用户的LinkedIn帐户在LinkedIn中具有业务帐户的潜在客户表单管理员权限。

   ![](assets/linkedin-pages-to-capture.png)

1. 要接受默认的LinkedIn到Marketo字段映射，只需单击 **创建**. 如果要更改默认字段映射、删除字段映射或添加新字段映射，可通过以下模式按字段执行此操作。

   >[!CAUTION]
   >
   >Marketo支持将两个LinkedIn字段映射到单个Marketo字段， **但只有** 两个LinkedIn字段不是同一表单。 如果将同一LinkedIn表单中的两个字段映射到单个Marketo字段，则用户可能无法输入您的Marketo数据库。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >仅已保存到的LinkedIn字段 [表单模板](https://www.linkedin.com/help/lms/answer/79634) 在LinkedIn促销活动管理器中，将显示为可映射到Marketo字段的LinkedIn字段。

   ![](assets/linkedin-installed-services.png)

干得好！ 在LinkedIn端运行成功的营销活动时，提交LinkedIn Lead Gen表单的人员将开始流入Marketo。

>[!NOTE]
>
>您只能授权单个LinkedIn用户帐户。 如果您有多个要链接到Marketo的业务帐户，请确保正在授权的用户的LinkedIn帐户具有LinkedIn中业务帐户的潜在客户表单管理员权限。

>[!MORELIKETHIS]
>
>[在智能营销活动中使用LinkedIn潜在客户表单过滤器和触发器](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
