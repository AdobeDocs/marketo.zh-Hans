---
description: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署步骤2（共3步） — Marketo文档 — 产品文档
title: 安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署步骤2（共3步）
source-git-commit: 7b1f0d0d45bbfe3d8b781282e0a4ef1884a2bf40
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 第2步（第3步）：设置Marketo Dynamics（2016年内部部署/Dynamics 365内部部署）{#step-of-set-up-for-marketo-on-premises-2016}

完成上述步骤的工作非常出色。 让我们继续过去。

>[!PREREQUISITES]
>
>[安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署步骤1（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## 分配同步用户角色 {#assign-sync-user-role}

将Marketo同步用户角色仅分配给Marketo同步用户。 您无需将其分配给任何其他用户。

>[!NOTE]
>
>这适用于Marketo版本4.0.0.14及更高版本。 对于早期版本，所有用户都必须具有同步用户角色。 要升级您的Marketo，请参阅 [升级适用于Microsoft Dynamics的Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>同步用户的语言设置 [应设置为英语](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. 在 **设置**，单击 **安全性**.

   ![](assets/assign1.png)

1. 单击 **用户**.

   ![](assets/assign2.png)

1. 您将在此处看到用户列表。 选择专用的Marketo同步用户，或联系您的 [Active Directory联合身份验证服务](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS)管理员，为Marketo创建专用用户。

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. 选择同步用户。 单击 **管理角色**.

   ![](assets/assign4.png)

   选中Marketo同步用户，然后单击确定。

   ![](assets/assign5.png)

   >[!TIP]
   >
   >如果看不到角色，请返回 [步骤1 - 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 并导入解决方案。

   >[!NOTE]
   >
   >同步用户在CRM中进行的任何更新都将 **not** 同步回Marketo。

## 配置Marketo解决方案 {#configure-marketo-solution}

快完了！ 在转到下一篇文章之前，我们只需完成一些最后的配置。

1. 在 **设置**，单击 **Marketo配置**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >如果Marketo配置缺失，请尝试刷新页面。 如果问题持续存在， [发布Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) 或尝试注销并重新登录。

1. 单击 **默认**.

   ![](assets/configure2.png)

1. 单击 **Marketo用户** 字段，然后选择同步用户。

   ![](assets/configure3.png)

1. 单击右下角的保存图标。

   ![](assets/configure4.png)

1. 单击 **发布所有自定义设置**.

   ![](assets/publish-all-customizations1.png)

## 继续执行步骤3之前 {#before-proceeding-to-step}

* 如果要限制同步的记录数， [设置自定义同步筛选器](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) 现在。
* 运行 [验证Microsoft Dynamics同步](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) 进程。 它验证初始设置是否正确完成。
* 在Microsoft Dynamics CRM中登录到Marketo同步用户。

>[!MORELIKETHIS]
>
>[安装Marketo for Microsoft Dynamics 2016/Dynamics 365内部部署步骤3（共3步）](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
