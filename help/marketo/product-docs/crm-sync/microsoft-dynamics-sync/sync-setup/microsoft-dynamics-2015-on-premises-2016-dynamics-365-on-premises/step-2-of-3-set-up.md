---
unique-page-id: 7504739
description: 安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤2（共3步）- Marketo Docs —— 产品文档
title: 为Dynamics 2015 On-Prem和2016 365 On-Prem安装Marketo步骤2（共3步）
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 步骤2（共3步）

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

完成前几步的工作做得不错。 让我们继续过去。

>[!PREREQUISITES]
>
>* [为Dynamics 2015 On-Prem和2016 365 On-Prem安装Marketo步骤1（共3步）](step-1-of-3-install.md)

>



## 分配同步用户角色{#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo Sync用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户必须具有同步用户角色。 要升级Marketo，请参阅[升级Microsoft Dynamics的Marketo解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**安全**。

   ![](assets/assign1.png)

1. 单击&#x200B;**用户**。

   ![](assets/assign2.png)

1. 您将在此看到一列表用户。 选择专用Marketo Sync用户或与[Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理员联系，为Marketo创建专用用户。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击&#x200B;**管理角色**。

   ![](assets/assign4.png)

   选中Marketto Sync User，然后单击OK。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果看不到该角色，请返回至第3步的[第1步（共3步），然后导入解决方案。](step-1-of-3-install.md)

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将&#x200B;**不**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们只有最后几段配置。

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**营销人员配置**。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在，[发布Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations)或尝试注销并重新登录。

1. 单击&#x200B;**默认**。

   ![](assets/configure2.png)

1. 单击&#x200B;**Marketo User**&#x200B;字段，然后选择同步用户。

   ![](assets/configure3.png)

1. 单击右下角的保存图标。

   ![](assets/configure4.png)

1. 单击&#x200B;**发布所有自定义**。

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

* 如果要限制同步的记录数，请立即[设置自定义同步筛选器](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
* 运行[验证Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。 它验证初始设置是否正确完成。
* 登录Microsoft Dynamics CRM中的Marketo Sync用户。

>[!NOTE]
>
>**相关文章**
>
>[为Dynamics 2015 On-Prem和2016 365 On-Prem安装Marketo步骤3（共3步）](step-3-of-3-connect.md)
