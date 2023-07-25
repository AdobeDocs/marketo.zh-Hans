---
unique-page-id: 3571816
description: 第2步（共3步） — 为Marketo配置同步用户（2013年内部部署） — Marketo文档 — 产品文档
title: 第2步（共3步） — 为Marketo配置同步用户（2013年内部部署）
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 第2步（共3步）：为Marketo配置同步用户（2013年内部部署） {#step-of-configure-sync-user-for-marketo-on-premises}

完成前面步骤的工作非常好，让我们继续介绍这些步骤。

>[!PREREQUISITES]
>
>[步骤1/3：在Dynamics中安装Marketo解决方案（2013内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)

## 分配同步用户角色 {#assign-sync-user-role}

仅将Marketo同步用户角色分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo插件版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅 [升级适用于Microsoft Dynamics的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用户的语言设置 [应设置为“英语”](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 下 **设置**，单击 **管理**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 选择 **用户**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您将在此处看到用户列表。 选择您的专用Marketo同步用户或联系您的 [Active Directory联合身份验证服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理员，以创建专用于Marketo的新用户。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击 ![](assets/image2015-3-26-11-3a16-3a22.png) 并选择 **管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Check **Marketo同步用户** 并单击 **确定**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果您看不到该角色，请返回 [步骤1/3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md) 并导入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将 **非** 已同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们仅提供了最后几段配置。

1. 下 **设置**，单击 **Marketo配置**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >如果 **Marketo配置** 缺失，请尝试刷新页面。 如果问题仍然存在， [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md) 再次尝试登录，或尝试注销并重新登录。

1. 单击 **默认**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 单击 **Marketo用户** 字段并选择同步用户。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 单击 ![](assets/image2015-3-13-15-3a10-3a11.png) 以保存更改。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 单击 **发布所有自定义项**.

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 进程。 它验证初始设置是否正确。
* 登录到Microsoft Dynamics CRM中的“Marketo同步用户”。

做得好！

>[!MORELIKETHIS]
>
>[步骤3/3：连接Marketo和Dynamics（2013年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2013.md)
