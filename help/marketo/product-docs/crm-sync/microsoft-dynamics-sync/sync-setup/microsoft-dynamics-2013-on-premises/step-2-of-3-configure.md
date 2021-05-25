---
unique-page-id: 3571816
description: 步骤2（共3步） — 为Marketo配置同步用户（2013年本地版） — Marketo文档 — 产品文档
title: 步骤2（共3步） — 为Marketo配置同步用户（2013年本地版）
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 步骤2（共3步）：为Marketo配置同步用户（2013本地版）{#step-of-configure-sync-user-for-marketo-on-premises}

完成上述步骤非常出色，让我们继续完成此步骤。

>[!PREREQUISITES]
[步骤1（共3步）：在Dynamics（2013本地版）中安装Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)>
>

## 分配同步用户角色{#assign-sync-user-role}

将Marketo同步用户角色仅分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
这适用于Marketo插件版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅[升级适用于Microsoft Dynamics的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

>[!IMPORTANT]
同步用户[的语言设置应设置为English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)。

1. 在&#x200B;**Settings**&#x200B;下，单击&#x200B;**Administration**。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 选择&#x200B;**用户**。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您将在此处看到用户列表。 选择您的专用Marketo同步用户或联系您的[Active Directory联合身份验证服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理员以创建专用于Marketo的新用户。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击![](assets/image2015-3-26-11-3a16-3a22.png)并选择&#x200B;**管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 检查&#x200B;**Marketo同步用户**&#x200B;并单击&#x200B;**确定**。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   如果看不到该角色，请返回至[第1步（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)并导入解决方案。

   >[!NOTE]
   同步用户在CRM中进行的任何更新都将&#x200B;**不**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快完了！ 在转到下一篇文章之前，我们只需完成一些最后的配置。

1. 在&#x200B;**Settings**&#x200B;下，单击&#x200B;**Marketo配置**。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   如果&#x200B;**Marketo配置**&#x200B;缺失，请尝试刷新页面。 如果问题仍然存在，请[再次发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)，或尝试注销后再重新登录。

1. 单击&#x200B;**Default**。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 单击&#x200B;**Marketo User**&#x200B;字段，然后选择同步用户。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 单击右下角的![](assets/image2015-3-13-15-3a10-3a11.png)以保存更改。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 单击&#x200B;**发布所有自定义项**。

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

* 如果要限制同步的记录数，请[立即设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 运行[验证Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确完成。
* 在Microsoft Dynamics CRM中登录Marketo同步用户。

干得好！

>[!MORELIKETHIS]
[步骤3（共3步）：连接Marketo和Dynamics（2013年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
