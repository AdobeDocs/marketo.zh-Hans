---
unique-page-id: 7504739
description: 安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤2（共3步） — Marketo文档 — 产品文档
title: 安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤2（共3步）
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 第2步（共3步）设置Marketo for Dynamics（2015年On-Prem和2016年365年On-Prem）{#step-of-set-up-for-marketo-on-premises-and-365}

完成前几步的工作非常出色。 让我们继续经历这个。

>[!PREREQUISITES]
>
>[安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 分配同步用户角色{#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo 4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级Marketo，请参阅[升级Marketo Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**安全**。

   ![](assets/assign1.png)

1. 单击&#x200B;**用户**。

   ![](assets/assign2.png)

1. 您将在此看到一列表用户。 选择专用Marketo Sync用户或与[Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理员联系，为Marketo创建专用用户。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击&#x200B;**管理角色**。

   ![](assets/assign4.png)

   选中Marketo Sync用户，然后单击“确定”。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果看不到该角色，请返回至3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)的[步骤1并导入解决方案。

   >[!NOTE]
   >
   >同步用户在您的CRM中所做的任何更新都将&#x200B;**不会**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们只有最后几段配置。

1. 在&#x200B;**Settings**&#x200B;下，单击&#x200B;**Marketo Config**。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在，[发布Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)或尝试注销并重新登录。

1. 单击&#x200B;**默认**。

   ![](assets/configure2.png)

1. 单击&#x200B;**Marketo User**&#x200B;字段，然后选择同步用户。

   ![](assets/configure3.png)

1. 单击右下角的保存图标。

   ![](assets/configure4.png)

1. 单击&#x200B;**发布所有自定义项**。

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

* 如果要限制同步的记录数，[请立即设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 运行[验证Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确。
* 在Microsoft Dynamics CRM中登录Marketo Sync用户。

>[!MORELIKETHIS]
>
>[安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤3（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
