---
unique-page-id: 3571807
description: 步骤2（共3步）-在Dynamics（2011年内部部署）中设置Marketo Sync用户- Marketo Docs —— 产品文档
title: 步骤2（共3步）-在Dynamics（2011年内部部署）中设置Marketo同步用户
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# 第2步，共3步：在Dynamics（2011内部部署）{#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}中设置Marketo同步用户

完成前几步的工作非常出色，让我们继续完成这一步。

>[!PREREQUISITES]
>
>* [第1步，共3步：安装Marketo解决方案（2011内部部署）](step-1-of-3-install.md)

>



## 分配同步用户角色{#assign-sync-user-role}

将Marketo Sync用户角色仅分配给Marketo Sync用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo插件4.0.0.14版及更高版本。 对于早期版本，所有用户必须具有同步用户角色。 要升级Marketo，请参阅[升级Microsoft Dynamics的Marketo解决方案](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md)。

1. 在左下方的菜单中，选择&#x200B;**设置**。

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. 在树中，选择&#x200B;**管理**。

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. 选择&#x200B;**用户**。

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. 您将在此看到一列表用户。 选择您的专用Marketo同步用户或与[Active Directory联合身份验证服务(AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx)管理员联系，以创建专用于Marketo的新用户。 单击&#x200B;**管理角色**。

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. 选中&#x200B;**Marketto Sync User**&#x200B;并单击&#x200B;**确定**。

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >如果看不到该角色，请返回至第3步的[第1步（共3步），然后导入解决方案。](step-1-of-3-install.md)

   >[!NOTE]
   >
   >同步用户在CRM中所做的任何更新都将&#x200B;**不**&#x200B;同步回Marketo。

## 配置Marketo解决方案{#configure-marketo-solution}

快完成了！ 在转到下一篇文章之前，我们只有最后几段配置。

1. 选择&#x200B;**设置**。 然后在树中选择**Marketo配置**。

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >如果缺少Marketo配置，请尝试刷新页面。 如果问题仍然存在，[再次](step-1-of-3-install.md)发布Marketo解决方案或注销并重新登录。

1. 单击&#x200B;**默认**。

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. 单击![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. 在弹出窗口中，选择同步用户。 然后单击&#x200B;**确定**。

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. 单击&#x200B;**保存**&#x200B;以保存更改。

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. 单击&#x200B;**发布所有自定义**。

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3 {#before-proceeding-to-step}之前

    *如果要限制同步的记录数，请立即[设置自定义同步过滤器](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md)。
    *运行[验证Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)进程。它验证初始设置是否正确完成。
    *在Microsoft Dynamics CRM中登录Marketo Sync用户。

干得好！

>[!NOTE]
>
>**相关文章**
>
>[第3步，共3步：将Microsoft Dynamics与Marketo连接（2011年内部部署）](step-3-of-3-connect.md)

