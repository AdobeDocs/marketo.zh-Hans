---
unique-page-id: 3571816
description: 步骤2（共3步）-为Marketo配置同步用户（2013本地版）- Marketo文档——产品文档
title: 步骤2（共3步）-为Marketo配置同步用户（2013年内部部署）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# 第2步，共3步：为Marketo配置同步用户（2013本地）{#step-of-configure-sync-user-for-marketo-on-premises}

完成前几步的工作非常出色，让我们继续完成这一步。

>[!PREREQUISITES]
>
>* [第1步，共3步：在Dynamics（2013内部部署）中安装Marketo解决方案](step-1-of-3-install.md)


## 分配同步用户角色{#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo Sync用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo插件4.0.0.14版及更高版本。 对于早期版本，所有用户必须具有同步用户角色。 要升级Marketo，请参阅[升级Microsoft Dynamics的Marketo解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**管理**。

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. 选择&#x200B;**用户**。

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. 您将在此看到一列表用户。 选择您的专用Marketo Sync用户或与您的[Active Directory联合服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [管理员联系以创建专用于Marketo的新用户。](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击![](assets/image2015-3-26-11-3a16-3a22.png)并选择&#x200B;**管理角色**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. 选中&#x200B;**Marketto Sync User**&#x200B;并单击&#x200B;**确定**。

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >如果看不到该角色，请返回至第3步的[第1步（共3步），然后导入解决方案。](step-1-of-3-install.md)

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将&#x200B;**不**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们只有最后几段配置。

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**营销人员配置**。

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >如果&#x200B;**Marketo Config**&#x200B;缺失，请尝试刷新页面。 如果问题仍然存在，[请再次发布Marketo解决方案](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations)或尝试注销并重新登录。

1. 单击&#x200B;**默认**。

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. 单击&#x200B;**Marketo User**&#x200B;字段，然后选择同步用户。

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. 单击右下角的![](assets/image2015-3-13-15-3a10-3a11.png)以保存更改。

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. 单击&#x200B;**发布所有自定义**。

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

* 如果要限制同步的记录数，请立即[设置自定义同步筛选器](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 运行[验证Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确完成。
* 登录Microsoft Dynamics CRM中的Marketo Sync用户。

干得好！

>[!NOTE]
>
>**相关文章**
>
>* [第3步，共3步：Connect Marketo和Dynamics（2013年内部部署）](step-3-of-3-connect.md)

