---
unique-page-id: 3571816
description: 步骤2（共3步） — 为Marketo配置同步用户（2013年本地版） — Marketo文档 — 产品文档
title: 步骤2（共3步） — 为Marketo配置同步用户（2013年本地版）
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: f130fa1187ccead6573f76ff947e55d42f6962e4
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 步骤2（共3步）：为Marketo配置同步用户（2013本地版） {#step-of-configure-sync-user-for-marketo-on-premises}

完成上述步骤非常出色，让我们继续完成此步骤。

>[!PREREQUISITES]
>
>[步骤1（共3步）：在Dynamics（2013本地版）中安装Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)

## 分配同步用户角色 {#assign-sync-user-role}

将Marketo同步用户角色仅分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo插件版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅 [升级适用于Microsoft Dynamics的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用户的语言设置 [应设置为英语](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 在 **设置**，单击 **管理**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 选择 **用户**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您将在此处看到用户列表。 选择您的专用Marketo同步用户，或与您的 [Active Directory联合身份验证服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理员来创建专用于Marketo的新用户。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击 ![](assets/image2015-3-26-11-3a16-3a22.png) 选择 **管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 检查 **Marketo同步用户** 单击 **确定**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果看不到角色，请返回 [步骤1 - 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) 并导入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中进行的任何更新都将 **not** 同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完了！ 在转到下一篇文章之前，我们只需完成一些最后的配置。

1. 在 **设置**，单击 **Marketo配置**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >如果 **Marketo配置** 缺少，请尝试刷新页面。 如果问题持续存在， [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) 再次尝试注销然后重新登录。

1. 单击 **默认**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 单击 **Marketo用户** 字段，然后选择同步用户。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 单击 ![](assets/image2015-3-13-15-3a10-3a11.png) 中，以保存所做的更改。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 单击 **发布所有自定义设置**.

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 进程。 它验证初始设置是否正确完成。
* 在Microsoft Dynamics CRM中登录Marketo同步用户。

干得好！

>[!MORELIKETHIS]
>
>[步骤3（共3步）：连接Marketo和Dynamics（2013年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
