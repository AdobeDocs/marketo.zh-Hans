---
unique-page-id: 3571816
description: 步骤2（共3步） — 为Marketo配置同步用户（2013年内部部署） — Marketo文档 — 产品文档
title: 步骤2（共3步） — 为Marketo配置同步用户（2013年内部部署）
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 第2步，共3步：为Marketo（2013本地）{#step-of-configure-sync-user-for-marketo-on-premises}配置同步用户

完成前几步的工作很好，让我们继续完成。

>[!PREREQUISITES]
>
>[第1步，共3步：在Dynamics（2013年内部部署）中安装Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## 分配同步用户角色{#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo插件4.0.0.14版及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅[升级Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**管理**。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 选择&#x200B;**用户**。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您将在此看到一列表用户。 选择专用Marketo Sync用户或与[Active Directory联合身份验证服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理员联系，以创建专用于Marketo的新用户。](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击![](assets/image2015-3-26-11-3a16-3a22.png)并选择&#x200B;**管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 选中&#x200B;**Marketo Sync User**&#x200B;并单击&#x200B;**确定**。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果看不到该角色，请返回至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)的[步骤1并导入解决方案。

   >[!NOTE]
   >
   >同步用户在您的CRM中所做的任何更新都将&#x200B;**不会**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们只有最后几段配置。

1. 在&#x200B;**Settings**&#x200B;下，单击&#x200B;**Marketo Config**。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >如果缺少&#x200B;**Marketo配置**，请尝试刷新页面。 如果问题仍然存在，[请再次发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)或尝试注销并重新登录。

1. 单击&#x200B;**默认**。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 单击&#x200B;**Marketo User**&#x200B;字段，然后选择同步用户。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 单击右下角的![](assets/image2015-3-13-15-3a10-3a11.png)以保存更改。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 单击&#x200B;**发布所有自定义项**。

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

* 如果要限制同步的记录数，[请立即设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 运行[验证Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确。
* 在Microsoft Dynamics CRM中登录Marketo Sync用户。

干得好！

>[!MORELIKETHIS]
>
>[第3步，共3步：Connect Marketo和Dynamics（2013年内部部署）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
