---
unique-page-id: 12976798
description: 设置LinkedIn潜在客户群Forms - Marketo文档 — 产品文档
title: 设置LinkedIn潜在客户Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: e1254c8156557b27d066a4482076becbd03fc774
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 设置LinkedIn潜在客户Gen Forms {#set-up-linkedin-lead-gen-forms}

使用LinkedIn潜在客户Gen Forms在LinkedIn中运行广告营销活动并为Marketo生成潜在客户。

>[!NOTE]
>
>**需要管理员权限**

>[!NOTE]
>
>如果LinkedIn商机与Marketo中与使用公司API创建的公司记录关联的现有人员记录匹配，并且Marketo订阅未连接到CRM，则它不会Marketo Engage。

1. 转到Marketo **管理员**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到 **启动点**，单击 **新建** 并选择 **新建服务**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 输入 **显示名称** 对于您的服务，选择 **linkedIn潜在客户** 服务，然后单击 **下一个**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo在同一浏览器中打开一个新选项卡，并执行以下操作 [linkedin.com](https://www.linkedin.com). 使用要用于集成的帐户登录LinkedIn。

   >[!NOTE]
   >
   >linkedIn帐户需要访问您为其创建赞助营销活动的所有LinkedIn业务帐户。

   ![](assets/linkedin-login.png)

1. 登录LinkedIn后，请返回Marketo并单击 **授权**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. 出现提示时，单击 **允许** ，以接受将Marketo应用程序安装到LinkedIn中。

   ![](assets/linkedin-marketo-allow.png)

1. 您会发现您现在已获得授权。 单击&#x200B;**下一步**。

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >该服务在获得授权后一年自动过期。 要重新获得访问权限，只需单击 **重新授权**. 根据浏览器设置，您可能需要重新输入LinkedIn密码。

1. 选择您希望LinkedIn潜在客户可以进入Marketo的帐户，然后单击 **下一个**.

   >[!TIP]
   >
   >如果您看不到所需的业务帐户，请确保已授权用户的LinkedIn帐户对LinkedIn中的业务帐户具有潜在客户一般表单管理员权限。

   ![](assets/linkedin-pages-to-capture.png)

1. 要接受默认的LinkedIn到Marketo字段映射，只需单击 **创建**. 如果要更改默认字段映射、删除字段映射或添加新字段映射，可以通过以下模式基于每个字段执行此操作。

   >[!CAUTION]
   >
   >Marketo支持将两个LinkedIn字段映射到一个Marketo字段， **但只有在** 两个LinkedIn字段不在同一表单上。 如果将同一LinkedIn表单中的两个字段映射到单个Marketo字段，则用户可能无法输入Marketo数据库。

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >仅限已保存至的LinkedIn字段 [表单模板](https://www.linkedin.com/help/lms/answer/79634) 在LinkedIn中，Campaign Manager将显示为可映射到LinkedIn字段的Marketo字段。

   ![](assets/linkedin-installed-services.png)

做得好！ 当您在LinkedIn端成功开展营销活动时，提交LinkedIn潜在客户群表单的人员将开始流入Marketo。

>[!NOTE]
>
>您只能授权一个LinkedIn用户帐户。 如果您有多个要链接到Marketo的业务帐户，请确保该用户获得授权的LinkedIn帐户对LinkedIn中的业务帐户具有“潜在客户一般表单管理器”权限。

>[!MORELIKETHIS]
>
>[在Smart Campaign中使用LinkedIn Lead Gen表单过滤器和触发器](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
