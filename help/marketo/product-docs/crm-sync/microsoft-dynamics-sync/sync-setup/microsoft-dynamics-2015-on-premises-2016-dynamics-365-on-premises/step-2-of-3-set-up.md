---
unique-page-id: 7504739
description: 安装Marketo for Dynamics 2015 On-Prem和2016 365 On-Prem步骤2（共3步）- Marketo Docs —— 产品文档
title: 为Dynamics 2015 On-Prem和2016 365 On-Prem安装Marketo步骤2（共3步）
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# 步骤2（共3步）

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

完成前几步的工作做得不错。 让我们继续过去。

>[!PREREQUISITES]
>
>* [为Dynamics 2015 On-Prem和2016 365 On-Prem安装Marketo步骤1（共3步）](step-1-of-3-install.md)

>



## 分配同步用户角色 {#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo Sync用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户必须具有同步用户角色。 要升级Marketo，请参 [阅升级Microsoft Dynamics的Marketo解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在“设 **置**”下，单 **击“安全**”。

   ![](assets/assign1.png)

1. 单击“ **用户**”。

   ![](assets/assign2.png)

1. 您将在此看到一列表用户。 选择专用Marketo Sync用户或与Active Directory Federation Services( [ADFS](https://msdn.microsoft.com/en-us/library/bb897402.aspx))管理员联系，为Marketo创建专用用户。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击 **管理角色**。

   ![](assets/assign4.png)

   选中Marketto Sync User，然后单击OK。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果看不到该角色，请返回第1步(共 [3步)并导](step-1-of-3-install.md) 入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都 **不会** 同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们只有最后几段配置。

1. 在“设 **置**”下，单 **击“Marketo配置”**。

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在， [请发布Marketo Solution](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) ，或尝试注销并重新登录。

1. 单击 **默认**。

   ![](assets/configure2.png)

1. 单击“Marketto **用户** ”字段，然后选择同步用户。

   ![](assets/configure3.png)

1. 单击右下角的保存图标。

   ![](assets/configure4.png)

1. 单击“ **发布所有自定义**”。

   ![](assets/publish-all-customizations1.png)

## 在继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数，请立 [即设置自定义同步筛选器](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 。
* 运行验 [证Microsoft Dynamics同步](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 。 它验证初始设置是否正确完成。
* 登录Microsoft Dynamics CRM中的Marketo Sync用户。

>[!NOTE]
>
>**相关文章**
>
>[为Dynamics 2015 On-Prem和2016 365 On-Prem安装Marketo步骤3（共3步）](step-3-of-3-connect.md)
